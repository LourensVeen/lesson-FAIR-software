---
title: "Add a License"
teaching: 15
exercises: 15
questions:
- "Why is a license important?"
- "When is a license important?"
- "How to choose a license?"
- "How does my license interact with an external library/package and its license"
objectives:
- "Learn about software licenses"
- "Add a license to a GitHub repository"
keypoints:
- "It is important to add an open-source license to make your code open."
- "There are several common licenses that have different permissiveness."
- "Under the surface it is more complicated, so take the recommended path."
---

> ## [Recommendation 2](https://fair-software.eu/recommendations/license)
>
> Add a license.
{: .callout}
![recommendation2]({{ page.root }}/fig/recommendation2.png)

*Disclaimer: This topic concerns law and can have serious repercussions. If you have a specific question ask an expert. 
This text is intended to give a short overview of licensing and is not legal counsel. For the purpose of education content is simplified. Do not soley base your decisions on this text.
*
## Why a license is important

Any creative work (including software) is automatically protected by copyright.
Even when the software is available via code sharing platforms such as GitHub,
no one can use it unless they are explicitly granted permission.
This is done by adding a software license, which defines the set of rules
and conditions for people who want to use the software.

Be aware that you, as the developer of a given piece of software,
may not be the copyright holder of the code you write. Often, the copyright
holder of the work is the employer (or hiring party) and not the author of the work.
If you are not the copyright holder you cannot simply license the code. 
Inform yourself of your institute's policy before putting code into the open.

> ## Stack overflow
>
> Suppose you wrote a small code snippet and want to share it with the rest of your research group. 
> While writing the code, you copied a couple of snippets from Stack Overflow. 
> What do you have to not get into trouble over copyright infringement?
> > ## Solution
> >
> > Read the [Stack Overflow post](http://meta.stackexchange.com/questions/271080/the-mit-license-clarity-on-using-code-on-stack-overflow-and-stack-exchange)
> > Code snippets published 01.02.2016 are published under the MIT license, but you do not have to add the MIT license. A link to the post is enough as attribution.
> {: .solution}
>
{: .discussion}

## Choose a license

We ask you to use one of the common licenses. Because these
were written by lawyers, the license text is precise in expressing
its terms. While that carries the unfortunate side effect of being lengthy and difficult
to understand, the widespread use of the popular licenses means that
there is a larger number of people who understand how the letter of
the law should be interpreted. 

There are several websites that can help you choose a license:

- [choosealicense.com](https://choosealicense.com/): helps to choose an open-source license.
- [tldrlegal.com](https://tldrlegal.com/): summarizes what is allowed and not allowed under a given license.

The 3 main rules of choosing a license:

- You have to be the owner of the code or have the owners' approval. Otherwise, you cannot do it.
- Choose a common license. People know those and understand what they mean. Nobody will spend hours and lawyers on your license to figure out what it means.
- Do not ever modify a license text. A modified license is a new license so more lawyers, time and money. 

## Permissive and copyleft licenses

The open-source licenses can be broadly separated into two categories: permissive and copyleft. 
The major difference is copyleft licenses require you to open-source your derived work under the same license. What counts as a derived work depends a bit from license to license but certainly if you take a code and modify it and you want to distribute it in any way you have to open-source it under the same license. 

Permissive licenses do not require that. People can more or less do whatever they want with the code, as long they attribute it to you and leave the license in that code and do not complain when it breaks something.

Copyleft licenses require people to release their source code under the same conditions to the world if they want to share it at all. Permissive licenses do not. Copyleft licenses prevent people form just taking the code modifying it and then making a profit. That also includes yourself, if you are not the sole copyright holder. 

Companies do like permissve licenses more, so if you want commerical contributions to your code a permissve license might be advantageous. On the other hand the linux kernel uses a copyleft license and has many commercial contributors. 

License compatibility can also impact your choice of license.

## License compatibility

Today most software depends on external libraries, modules or packages, which have their own licenses. How do these licenses influence or limit your choice of the license?
This is the realm of license compatibility and it is complictated, because it depends on 
- how you package your software
- how integrated the library is in your code
- what the specific license of that library requires
- what the dependencies of that library require

Among permissive licenses you will generally not have many problems, but copyleft licenses make things more difficult
A nice overview is found [in the Turing Way Boook](https://the-turing-way.netlify.app/reproducible-research/licensing/licensing-software.html).

[FOSSA](https://fossa.com/?ref=tldrlegal) is a tool which for some programming languages helps you to scan and ascertain that all requirements are met.

Also, think about the data you might ship together with your project because data has copyright too. So check your data.

## Re-licensing your code

What if you picked the wrong license 5 years ago and now want to change that? If you are the only and single copyright holder of the code, you can change the license for the next version. Old releases of your code will still be available under the old license. If you are not the sole copyright holder you have to get the approval of all copyright holders, who made a significant contribution to the code.

> ## Choosing a license for a project at the university
>
> Suppose you write code for a project at the university.
> Open sourcing software may not yet be a common practice in your community,
> and there is no clear standard software license to use. What steps will you take?
>
{: .discussion}

> ## Add a license to your GitHub repository
>
> Go to your new repository on GitHub and add a license.
>
> > ## Solution
> >
> > Follow the instructions
> > on the [GitHub help pages](https://docs.github.com/en/github/building-a-strong-community/adding-a-license-to-a-repository).
> {: .solution}
{: .challenge}

{% include links.md %}
