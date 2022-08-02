---
title:  "Comparing lambda expressions in four JVM-hosted languages"
description: "Encompasses understanding how science works, how to find resources, and how to cite them. LaTeX centered."
date: "2020-05-08T19:25:30+02:00"
publishDate: "2020-05-08T19:25:30+02:00"
---

[![wikipedian protester](https://imgs.xkcd.com/comics/wikipedian_protester.png)](https://xkcd.com/285/)

<script>
MathJax = {
  tex: {
    inlineMath: [['$', '$'], ['\\(', '\\)']]
  },
  svg: {
    fontCache: 'global'
  }
};
</script>
<script type="text/javascript" id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-svg.js">
</script>

## Preamble: understanding how science works

This may sound surprising, but I learnt what a scientific paper actually was during my master degree,
when... well, when I published my first paper, basically.
At least in my university, nobody cared spending time to explain us how the publication of scientific results worked,
it is an information that somewhat boils up from the context,
with the final result that for many bachelors there's not much of a difference in reliability between an article on a blog and a paper published on a high level journal.

So, the very first step to be able to prepare a decent bibliography for your thesis is understanding how scientific stuff gets written and published.
If you got enough time, I suggest the [Science 101][Science 101] course from Berkeley.
If you must run and/or you know exactly how science works, at least make sure that you understand the [basics of peer review][Peer Review].


## Recognizing scientific papers

Once you understand that you need to tell scientific papers apart from other resources,
the first thing you need is a way of recognizing if some document is a scientific paper.

There is (almost) no way to do so by just looking at the document: Internet is flooded with
pdfs that look just like legitimate papers,
but are actually drafts or unrevised technical reports of some sort.

Once you find a resource that you want to cite, verify that it is actually a paper.
One way to do so is by searching for its title and authors.
If it is a scientific paper, you should be able to find the scientific journal
where it has been published.
A very useful information you should try to obtain is the [Digital Object Identifier (DOI)][DOI] of the work. If you manage to find it, you can immediately [resolve it to the actual URL of the published paper][URL].
While finding the DOI for a work does not guarantee per se that the work is a scientific paper,
not finding a DOI associated with a work should trigger an alarm:
every decent venue binds the published work with a DOI.

Once you got a handle on where the paper has been published,
you should try to understand how reliable is what you have found.
Reliability of different sources varies among disciplines,
here I will discuss how it works for computer science and engineering.

You may find that your work has been published in:

* a scientific journal, you can recognize the journal name and find its website where all the issues and volumes should be listed;
* A conference proceedings, a collection of works presented at some conference, whose name is typically in a form like "Proceedings of the x-th conference/workshop on some argument";
* On [Arxiv][Arxiv] or similar e-print hosting system


### Making sure that a journal publication is decent

Finding the publication on a journal is a good sign.
Typically, it is the venue where the peer review process is stricter
(although some conferences can be very tough to get into).
One important exception are the so-called predatory journal, or pay-per-publish.
These are journals that mock the peer-review process and then publish papers asking authors for money.
Articles published there have no more value than a post on Facebook,
so it's a good practice to check that the journal is actually a legitimate one.
To do so, you can check if it is listed in one of the [lists of predatory journals][Predatory Journals List].


### Evaluating the quality of a conference

Conference proceedings can host very high or very low quality papers.
This lagerly depends on who participates the conference, how big is the community behind it,
how well regarded it is, and how hard is to get some work past the review process.
High level conferences can be tougher than most journals;
on the other side of the spectrum, often workshops get organized with the primary goal of stimulating
a scientific discussion, hence with a very lightweight review process,
as the event goal is to kickstart the production of novel science and ideas rather than presenting
some finished or almost-finished work.

There's no easy way to tell conferences apart by quality simply looking at their name.
As a rule of thumbs, if "workshop" is in the title the publications are probably somewhat less valuable.


### Pre-prints (e.g., Arxiv)

[Arxiv][Arxiv] is a service that allows for sharing *pre-prints* of a scientific paper.
A pre-print is a document that may one day become a paper, but whose peer-review process has not been concluded.
It is possible that the work has very serious flaws and will never get published.
When possible, citing pre-prints should be avoided.

Many scientists publish pre-prints to try to contribute quickly to hot topics,
or because they believe the work needs to get reference even though the review process is not yet concluded.
The unfortunate fact that peer review can take months or years to complete does not help.


## Searching for scientific papers

You should now be able to distinguish scientific papers from other kinds of document,
and understand (more or less) how reliable a paper seems to be.
It is now time to search.
Searching the keywords relevant for you on Google is probably not the best choice for a thesis.
Wikipedia, newspapers, and even blogs may easily appear first in the proposed results.
For this reason, there are dedicated search engines.

One is [Google Scholar][Google Scholar].
Typing your keywords there have a good chance to propose you actual scientific papers (you still need to double check, though).

There are also other engines with better guarantees, such as [Scopus][Scopus].
If you are a student at University of Bologna, you should be able to have access to the search for documents.
Scopus tracks a number of certified sources, hence the papers found there are usually of good value.

There are other very important search engines (PubMed and Web of Science above all),
but they rarely host papers relevant for Computer Science and Engineering that are not on Scopus.
Should you need something about medicine, however, PubMed is probably the search engine to use.


## Accessing scientific papers

By this point, you may have noticed that you can't access many scientific works.
They are beyond paywalls,
as selling access to scientific knowledge is the way publishers get money out of the publishing process.
There is no easy *and legal* way around it.
If you are connected to the university network, you should have access to most of them.
If you are not, it is possible that your supervisor can access them, and send you a copy, try to contact hir.
Of course, [Sci-Hub](https://sci-hub.tw/), [Library Genesis](https://libgen.is/) and similar services that provide open access to scientific research are not legal and are mentioned here solely for the sake of completeness.

## Obtaining BibTeX entries

The best way to reference a paper in $\LaTeX$ is by using BibTeX.
It allows to collect all the information about the references in a `.bib` file,
and then reference them in text by using `\cite{bibtexEntryName}`.
The typesetter formats them coherently for you.
Wonderful.

A bibtex entry in your `.bib` file is an object looking like this:

```latex
@article{aggregate-programming,
  author    = {Jacob Beal and
               Danilo Pianini and
               Mirko Viroli},
  title     = {Aggregate Programming for the Internet of Things},
  journal   = {IEEE Computer},
  volume    = {48},
  number    = {9},
  pages     = {22--30},
  year      = {2015},
  url       = {https://doi.org/10.1109/MC.2015.261},
  doi       = {10.1109/MC.2015.261},
  timestamp = {Mon, 05 Jun 2017 20:51:35 +0200},
  biburl    = {https://dblp.org/rec/journals/computer/BealPV15.bib},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```

It's just a collection of the information we have about some work,
that $\LaTeX$ will be using to format our citation correctly.
The bad news is that it's pretty verbose,
and there is a ton of information for each work you may need to cite;
the good news is that you do not need (and should not actually)
write BibTeX entries yourself: you can find them ready for use.

In my opinion, the best source for bibtex of documents in computer science and engineering
is [DBLP][DBLP].
Search by the name of one of authors of the paper you want to cite,
find hir, find the work in the page, and under *export record*
you'll find a `BibTeX` button.
It will generate a BibTeX entry for you.
There is one only thing to pay attention to:
DBLP uses `crossref` to connect scientific works to their venues.
You have two choices here:

1. copy only the entry of the work, ignore the venue, and delete the `crossref` line
2. copy everything, but make sure you do not repeat the entry of the venue multiple times into your `bib` file.

Both strategies are fine for a thesis.

If you need to cite a paper that's not on DBLP,
the second best tool I want to recommend is [doi2bib](https://www.doi2bib.org/).
It's very very easy: open the page, past the DOI, get the bib.
Results may vary (it's not as surgically precise as DBLP),
but it usually provides very good entries.

If you need to cite an RFC,
[this tool](http://notesofaprogrammer.blogspot.com/2014/11/bibtex-entries-for-ietf-rfcs-and.html)
should be able to generate BibTeX entries.


## Cite all the stuff

You now have scientific papers and possibly other resources that you want to refer to in your work.
However, you also know that not every document has the same dignity.
A paper published on a top journal,
a pre-print from Arxiv,
a RFC,
a link to the website of some company,
and an article from an online newspaper
have different value and should be treated differently.

In the following,
I suggest how to organize the bibliographic references of your thesis.
There is no rule carved in stone for this, different authors may use different approaches.
However, in case I'm going to be your supervisor (and if you are reading this from by blog that's very likely), I will enforce these rules.

**Objects with a DOI**

Objects with a DOI should go in bibliography.

**RFCs and the like**

RFCs and other reviewed and official documents,
documenting protocols or procedures,
should go in bibliography.

**Links to online newspapers**

Citing well-known journalistic sources with an online version is fine,
but they should not go in bibliography.
You should first protect them from the ephimeral nature of the Internet by [archiving them](http://archive.is/),
then use `\footnote{\url{archivedUrl}}` to reference them.
Links to Wikipedia, documentation pages, or blogs should follow the same procedure.

**Links to companies, products, repositories**

In this case there is little reason to archive,
the links should be stable and if they are not...
well, the company probably defaulted.
You can link them in the footnote without archiving the page.

#### Style suggestions

* Citation go before punctuation, space-separated from the previous text. In order to prevent newlines between a sentence and a citation, separate the `\cite` command with a tilde: e.g.,

```latex
the field calculus~\cite{hofc} is universal~\cite{fc-universality}.
```

* Footnotes go before punctuation, without spaces

```latex
Kotlin\footnote{https://kotlinlang.org/} is a programming language
by JetBrains\footnote{https://www.jetbrains.com/}.
```

[Arxiv]: https://arxiv.org/
[DOI]: https://www.doi.org/
[DBLP]: https://dblp.uni-trier.de/
[Google Scholar]: https://scholar.google.com/
[Peer Review]: https://undsci.berkeley.edu/article/howscienceworks_16
[Predatory Journals List]: https://predatoryjournals.com/journals/
[Science 101]: https://undsci.berkeley.edu/article/intro_01
[Scopus]: https://www.scopus.com/
