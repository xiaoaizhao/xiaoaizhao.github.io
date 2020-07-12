---
layout: post
title: Academic writing in markdown - why it's the way forward and you should definitely give it a try
tags: [Academic Writing, Markdown, BibTeX, Pandoc]
hide_title: false                                  # Hide the title when displaying the post, but shown in lists of posts
feature-img: "assets/img/pexels/travel.jpeg"              # Add a feature-image to the post
thumbnail: #"assets/img/thumbnail/sample-th.png"   # Add a thumbnail image on blog view
color: rgb(132,166,176) #rgb(80,140,22)                             # Add the specified color as feature image, and change link colors in post
bootstrap: false
---

When it comes to academic writing - I'm using this general term to refer to writing journal articles, research grant proposals and book chapters, there is almost never a debate on what technical tool to use and how to get started. You open a new Word document and type away, at least this has been the status in the biomedical research field for a long time. Biologists comply to this norm for a few reasons: 1) There is virtually no barrier of entry - everyone knows how to navigate Microsoft Word to some degree. Sure, you might need to learn a few functions that are unique to academic writing, namely inserting and managing reference citations, but you pick it up along the way. 2) It becomes a standard in the field when scientific journals reinforce the use of Word document. Most of  journals across all tiers in biomedical research field requires manuscript submission in Word. Even when they are open to papers prepared in LaTeX, they require these manuscripts to be converted to Word document at some point during the editorial process, for instance, at [time of submission](https://www-sciencemag-org.stanford.idm.oclc.org/authors/science-information-authors) or [after acceptance](http://www.nature.com.stanford.idm.oclc.org/nature/for-authors/formatting-guide). 3) Perhaps the strongest force contributing to this norm is just the fact that _everyone is using Word._ Contrary to common perceptions of scientist who is hunched over writing by him/herself, academic writing is and has been incredibly collaborative. Research projects that involve multiple scientists working together have more than one authors contributing to paper-writing. It helps that everyone is using the same software and can work on the document together. Even in the cases of "Single-author writing" such as drafting grant proposals, you constantly seek comments/feedbacks from your peers and mentors. This makes features such as track change and adding comments an integral part of the process.

With everything mentioned so far, going with Word sounds like a no-brainer. For better or worse, Word and EndNote are provided by most universities and research institutions for free to researchers. However, both of these softwares are proprietary, which means they can't easily be viewed or edited by other programs. In another word, once you start using them, you are stuck with them.<!-- the previous sentence needs to be polished--> Now, recall the countless times when suddenly Word crashes as soon as you try to use EndNote. Or when your co-authors made a change in a shared Word document but it shows up incorrectly on your end. Or the most concerning of all - references were missing or linked incorrectly because different versions of softwares were involved. In those moments, do you wish you could have a system that _just works_, I certainly do. Almost all of these problems can be attributed to version and operating system incompatibility in one or more of these softwares. They cause everything from minor annoyances to serious erratum, and it's precisely what motivated me to spend some time looking for a better alternative.

Taking into account all considerations, the ideal infrastructure for academic writing in the biomedical research field (and many other scientific fields) should meet the following criteria:

##### Required

1. Easy to learn and easy to transition for people who have been exclusively using Word previously.
2. Ability to integrate and stylize citations.
3. Flexible to convert to specific file format required for journal submission.
4. Amenable to collaborative writing and can incorporate edits and comments.

##### Preferred

1. Platform agnostic (able to run on MacOS, Windows, Linux and mobile OS).
2. Future proof. Failure or success of any given company does not hijack the entire workflow. In another word, you do not have to go back to the drawing board 5-10 years down the road just because the company who makes your favorite text-writing software decides to disappear.

There is an obvious contender that might come to your mind. That's exactly why [LaTeX](https://www.latex-project.org/) has been widely adopted in many other research fields such as math and physics. In biology however, LaTeX meets **almost all** requirements **except the very first one**. The learning curve is just not trivial for a lot of wet biologists who have limited experience in coding. It is especially hard to justify the cost of learning when considering that paper writing in biology don't take enough advantage of star features in LaTeX, such as the powerful capability to write [inline math](https://www.overleaf.com/learn/latex/mathematical_expressions). Since typesetting is mostly taken care of by journals, beautiful typesetting by LaTeX also becomes a moot point. However it's worth mentioning that in the new age of preprint servers, a nicely typeset article will make your paper instantly more readable and stand out from a sea of double-spaced manuscript directly exported from Word. With that said, let's keep LaTeX on the table and may be we can revisit some time down the road.

Enter [markdown](https://en.wikipedia.org/wiki/Markdown). In the simplest term, it's writing in plain-text and use basic syntax for formatting. To give you a better idea, I'm listing a few of the most frequently used syntax that comes to mind in biomedical academic writing. There are many great resources online such as this [original guideline](https://daringfireball.net/projects/markdown/syntax) that will give you a better picture of what markdown can offer in its fullest potential.

|   Format style    |           Example           |                   Output                    |
| :---------------: | :-------------------------: | :-----------------------------------------: |
|     **Bold**      |     `**This is bold**`      |              **This is bold**               |
|     *Italic*      |     `*This is italic*`      |              *This is italic*               |
| ~~Strikethrough~~ | `~~This is strikethrough~~` |          ~~This is strikethrough~~          |
|    Superscript    |  `Your Favorite Gene^+/-^`  |      Your Favorite Gene<sup>+/-</sup>       |
|     Subscript     | `Cells need O~2~ and CO~2~` | Cells need O<sub>2</sub> and CO<sub>2</sub> |

I will now spend some time and show you just how writing in markdown fulfills **all the required and desired criteria** we set out earlier.

As you can hopefully see, it's really easy to get started writing in markdown. Formatting syntax is not intimidating, and very minimal so it won't break your writing flow. Besides, thanks to its open format, **it can be viewed with any text editor**. Even more so, it gives you a wide range of options to choose your favorite markdown text editor. For example, [Typora](https://www.typora.io/) (my personal favorite) and [iA Writer](https://ia.net/writer) put writing experience front and center by creating a clean and distraction-free environment. [Atom](https://atom.io/) and [VS Code](https://code.visualstudio.com/) are geared towards programmers and provide versatile functionality. Whether you prefer open-source software or you value user experience above all else, there is a text editor for you.

To write in markdown means we also need to manage bibliography in markdown. That's where [BibTeX](http://www.bibtex.org/) comes in. Because it's also a plain-text file format like markdown, BibTeX works perfectly with markdown, even though it was originally created to be used alongside LaTeX. Many popular reference management softwares such as [Zotero](https://www.zotero.org/), [Mendeley](https://www.mendeley.com/) and EndNote all support exporting your existing library into BibTeX format, so you don't have to worry about re-creating your entire library from scratch.

```BibTeX
  @article{folchSimpleMethodIsolation1957,
  title = {A Simple Method for the Isolation and Purification of Total Lipides from Animal Tissues},
  author = {Folch, J. and Lees, M. and Sloane Stanley, G. H.},
  year = {1957},
  month = may,
  volume = {226},
  pages = {497--509},
  issn = {0021-9258},
  journal = {The Journal of Biological Chemistry},
  keywords = {Lipids,LIPIDS/determination},
  language = {eng},
  number = {1},
  pmid = {13428781}
}
```


This is what a typical entry in `.bib` file looks like, it consists of all tags necessary to generate bibliography in academic papers. The string after `@article{` in the first line is called citation-key. The way you insert a reference into your markdown document is by adding `@citation-key`, which is usually displayed as `[author][year]`. I use the [better BibTeX plugin for Zotero](https://retorque.re/zotero-better-bibtex/) which exports the citation-key as `[author][short_title][year]`(e.g. `@folchSimpleMethodIsolation1957`). To me the added short title provides significantly more context than just author name and year, it also makes it much easier to spot incorrect citations when writing and proof-reading. Before you ask, no, you don't have to manually type in the long string of citation-key, or even copy and paste. There are a number of ways to add BibTeX citation with auto-completion such that as you start typing in the first few characters of the citation-key, you will be prompted with a list of possible matching references, from which you can choose the correct one to insert. I use [Autocomplete-bibtex](https://atom.io/packages/autocomplete-bibtex) package for Atom, it's very easy to set up and works well. [Zettlr](https://www.zettlr.com/) is a markdown editor made with scientists in mind and even has citation auto-completion built-in, which makes it very attractive to people who are just transitioning from writing in Word.

With writing and bibliography all set up, we now need a magic wand that glues different parts together and I can't stress enough how important [Pandoc](https://pandoc.org/) is in making our new writing system exhilaratingly flexible and versatile. It first is a universal document converter. Remember how journals _love_ Word document? Pandoc offers conversion between markdown file with Word document and PDF, even LaTeX. It has more tricks up its sleeve by allowing you to apply any reference style you want and will render your manuscript with bibliography in desired style _and_ file format you specified for export. All you need to do is including this metadata header in the beginning of your markdown file. Pandoc will effectively understand the command to 1) link `My_paper.bib` reference library and 2) format bibliography according to a style specified by your journal of choice. There are over 9000 styles that you can [download](https://www.zotero.org/styles) which covers almost any journal you have in mind.

```` YAML
---
bibliography: My_paper.bib
csl: My_dream_journal.csl
---
````

Once we finished all of the writing and formatting, in order to qualify as a good writing system for academic writing, it must also have the ability for collaborative writing and editing. [Git](https://git-scm.com/) and [Github](https://github.com/) are such powerful tools that allow multiple people to work on the same file at the same time, compare different edits from all users and combine all changes together. It was designed for software developer, but again since we are exclusively working with plain-text files for writing and reference management, academic writing is a perfect use case for Git/Github. This topic deserves a separate post on its own, but for now just know that if you are willing to invest just enough to navigate a few basic commands in Git, it is much more powerful than any of these features you are used to and rely on, such as track change and commenting in Word.

Hope you can see by now that adopting markdown in academic writing workflow offers tremendous value. Not only does it meet all of the criteria we set out earlier, thanks to its plain-text open-format, one can easily work with it on any computer operating systems for a long time to come. It even works on [mobile systems](https://www.idownloadblog.com/2020/01/09/free-markdown-text-editors-iphone-ipad/) which are becoming the preferred writing medium for increasing number of people. Having a mentor or colleague who feels they live and breathe Word? Not to worry at all, thanks to the flexible system we just set up, it is easy enough to convert our writing to any format to their liking. I am well aware that the system will work the best when everyone is onboard. I don't know if and when the universal switch will happen, nor do I plan to hold my breath for it. In the mean time, I will continue to enjoy the liberating flexibility that system built with markdown, BibTeX and Pandoc offers - so long version incompatibility. I don't care if it's [EndNote crashing Word](https://community.endnote.com/t5/EndNote-General/EndNote-crashing-Word/td-p/153005) or [Word crashes on its own](https://docs.microsoft.com/en-us/office/troubleshoot/word/word-for-mac-crashes-or-quits). I'm no longer forced to interact with products that cause unnecessary headaches in my life, and I will focus my energy on writing and communicating research better than ever before.



-Xiaoai
