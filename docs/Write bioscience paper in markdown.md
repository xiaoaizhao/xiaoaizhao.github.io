## Academic writing in markdown language - why it's the way forward and you should definitely give it a try.



When it comes to academic writing - I'm using this general term to refer to writing journal articles, research grant proposals and book chapters, there is almost never a debate on what technical tool to use and how to get started. You open a new Word document and type away, at least this has been the status in the biomedical research field for a long time. Biologists comply to this norm for a few reasons: 1) There is virtually no barrier of entry - everyone knows how to navigate Microsoft Word to some degree. Sure, you might need to learn a few commands and functions that are unique to academic writing, namely inserting and managing reference citations (usually from EndNote or other citation management software), but you pick it up along the way. 2) It becomes a standard in the field when scientific journals reinforce the use of Word document. Most of  journals across all tiers in biomedical research field requires manuscript submission in Word. Even when they are open to papers prepared in LaTeX, they require these manuscripts to be converted to Word document at somepoint during the editorial process, for instance, at [time of submission](https://www-sciencemag-org.stanford.idm.oclc.org/authors/science-information-authors) or [after acceptance](http://www.nature.com.stanford.idm.oclc.org/nature/for-authors/formatting-guide). 3) Perhaps the strongest force contributing to this norm is just the fact that _everyone is using Word._ Contrary to common perceptions of scientist who is hunched over writing by him/herself, academic writing is and has been incredibly collaborative. Research articles which involve multiple scientists working together have more than one authors contributing to paper-writing. It helps that eveyone is using the same software and can work on the document together. Even in the cases of "Single-author writing" such as drafting grant proposals, you constantly seek comments/feedbacks from your peers and mentors. This makes features such as track change and adding comments an integral part of the process. 

With everything mentioned so far, sticking with Word sounds like a no-brainer. But more and more so I have begun to feel the painpoints that this system created in the writing process.<!-- the previous sentence needs to be polished--> Both Word and EndNote are proprietary softwares, which means they can't be viewed by other program  and they are not free. Usually it's a non-issue since they are provided by most universities and research institutions. However in this day and age when we are debating open access journals vs. traditional journals, a preference for transitioning over to open-source softwares for academic writing shouldn't simply be brushed over<!-- this is kind of a moot point now the correct word is open format vs. proprietary-->. But let's say you don't care about any of this, what about the countless times when suddenly Word crashes as soon as you try to use EndNote. Or when your co-authors made a change in a shared Word document but it shows up incorrectly on your end. Or the most concerning of all - references were missing or wrong because different versions of softwares were involved. Almost all of these problems can be attributed to version and operating system incompatibility in one or more of these softwares. They cause everything from minor annoyances to serious erratum, and it's precisely what motivated me to spend some time looking for a better alternative. 

Taking into account all considerations, the ideal infrastructure for academic writing specifically in the biomedical research field should meet the following criteria:

##### Required

1. Easy to learn and easy to transition for people who have been exclusively using Word previously.
2. Ability to integrate and stylize citations.
3. Flexible to convert to specific file format required for journal submission. 
4. Amenable to collaborative writing and can incorporate edits and comments.

##### Preferred

1. Platform agnostic (able to run on MacOS, Windows, Linux and mobile OS).
2. Future proof. Failure or success of any given company does not hijack the entire workflow. In another word, you do not have to go back to the drawing board 5-10 years down the road just because the company who makes your favorite text-writing software decide to go bankrupt.

There is an obvious contender that might come to your mind. That's precisely why [LaTeX](https://www.latex-project.org/) has been widely adopted in many other research fields such as  math and physics. In biology however, LaTeX meets **almost all** requirements **except the very first one**. The learning curve is just not trivial for a lot of wet biologists who have limited experience in coding before. It is especially hard to justify the cost of learning when considering that paper writing in biology don't take enough advantage of star features in LaTeX, such as the powerful capability to write [inline math](https://www.overleaf.com/learn/latex/mathematical_expressions). Since typesetting is mostly taken care of by journals, beautiful typsetting by LaTeX also becomes a moot point. However it's worth mentioning that in the new age of preprint servers, a nicely typeset article will make your paper instantly more readable and stand out from a crowd of double-spaced manuscript directly exported from Word. With that said, let's keep LaTeX on the table and may be we can revisit some time down the road.

Enter [markdown language](https://en.wikipedia.org/wiki/Markdown). In the simpliest term, it's writing in plain-text and use basic syntax for formatting. If the previous sentence doesn't mean anything to you, to give you a better idea, I'm listing a few of the most frequently used syntax that comes to mind in biomedical academic writing. There are many great rescources online such as this [original guideline](https://daringfireball.net/projects/markdown/syntax) that will give you a better picture of what markdown can offer in its fullest potential.

|   Format style    |           Example           |          Output           |
| :---------------: | :-------------------------: | :-----------------------: |
|     **Bold**      |     `**This is bold**`      |     **This is bold**      |
|     *Italic*      |     `*This is italic*`      |     *This is italic*      |
| ~~Strikethrough~~ | `~~This is strikethrough~~` | ~~This is strikethrough~~ |
|    Superscript    |  `Your Favorite Gene^+/-^`  |  Your Favorite Gene^+/-^  |
|     Subscript     |     `Cells need CO~2~`      |     Cells need CO~2~      |

I will now spend some time and show you just how writing in markdown fulfill **all the required and desired criteria** we set out earlier.

#### Easy to learn and easy to transition for people who have been exclusively using Word previously.

As you can hopefully see, it's really easy to get started writing in markdown. In addition to , the following features to be used for academic writing and 

-open format, use any editor you want. Typora iAwriter Atom Zettlr



#### Ability to integrate and stylize citations.

BibTex , all-in-one Zettlr

#### Flexible to convert to specific file format required for journal submission. 

Pandoc even to LaTeX, citation style

#### Amenable to collaborative writing and can incorporate edits and comments.

Git

in my opinion everyone, especially biologists should think about transitioning to writing  in markdown. 



