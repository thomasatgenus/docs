# Genus App Platform&reg; documentation contributor guide
This is the publically available documentation for the Genus App Platform published at [docs.genus.no](https://docs.genus.no).

Feel free to contribute! See [Ways to contribute](#ways-to-contribute) on how to do it.

See www.genus.no for more general information about our products and our company.

## Guidelines
* Keep the articles short and to the point.
* It is better to start out small and then iterate and evolve more content later.
* Commit consistent and complete articles. If it isn't possible, state clearly in the article that the content is unfinished. Please return to finish it as soon as possible.
* If you are trying to improve upon an article, but find it hard to describe the functionality, it may be Genus App Platform that needs improvement. Please let us know through your support channel!
* Use images sparingly, as these are hard to maintain over time. Put any images in the media subfolder of your article. If you are submitting a screen shot, make sure that it doesn't contain any customer specific information.
* If you are unsure of the article content, spelling, or otherwise, submit a pull request and our editors will help you out.
* Use [sentence case](https://en.wikipedia.org/wiki/Letter_case#Case_styles) almost everywhere, also in article main headings. The exception is proper nouns like those defined in the [Glossary](developers/defining-the-application-model/glossary.md) (Genus App Platform, Genus Apps etc). See example [here](https://github.com/GenusAS/docs/blob/master/developers/installation-and-configuration/system-requirements.md).
* Use hyphens (-) in article file and folder names, since the markdown previewers do not like spaces in article cross references.

## Transition period guidelines
We are currently in a transition period from our old documentation structure. Most of the old documentation has been converted automatically, but a couple of things remain. We appreciate your assistance with the following:
* Change the term "Application" to "App".
* Convert Html tables to [Markdown tables](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#tables). (Who completes [this](developers/keyboard-shortcuts.md) article?)
* Article main headers are supposed to be [H1](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#headers) (`# H1`), subheadings H2 (`## H2`) etc. Example [here](developers/defining-the-application-model/general-settings/data-sets.md).
* Change header capitalisation to [sentence case](https://en.wikipedia.org/wiki/Letter_case#Case_styles). Example [here](developers/installation-and-configuration/system-requirements.md).
* Automatically converted media files have ended up with a GUID file name like "ID3C264089A1BE49C2.IDC90AF0450EE242F6.png". Please change to a "normal" descriptive name - or simply delete the file if it is a screen dump that is hard to maintain (ref. the guidelines regarding screen shots above).

## Ways to contribute
You can submit updates to the Genus App Platform documentation as follows:
* If your are making small changes, like adjusting content of an article, use the [GitHub](https://github.com/GenusAS/docs) user interface. Either find the article in this repository, or visit the article on [docs.genus.no](https://docs.genus.no) and click the "Improve this doc" link, which will take you to the article in GitHub.
* All articles are written in [markdown](https://en.wikipedia.org/wiki/Markdown). You may contribute directly by submitting pull requests. Employees of Genus may commit directly. All pull requests and commits are reviewed by the internal Genus editorial board.
* If you are making substantial changes to an existing article or a series of articles or adding several new articles, you may want to [do the work locally on your computer](editing-docs-locally.md).

Note that a commit automatically will trigger a rebuild of the docs site, which will be available at [docs.genus.no](https://docs.genus.no) in about 5 minutes.

Please provide any commit comments in English. It is not necessary to provide commit comments for minor changes like correcting spelling errors or similar.

## How to use markdown
All the articles in the repository use GitHub and DocFX flavored Markdown. Here is a list of resources.
* [Markdown basics](https://help.github.com/articles/markdown-basics/) (from GitHub)
* [DocFX flavoured Markdown](https://dotnet.github.io/docfx/spec/docfx_flavored_markdown.html)
* [Markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* [Printable Markdown cheatsheet](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)