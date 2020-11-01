# Basic
- Technical writing need to be "formal" - pay attention to important information and polish to details
- Technical documentation should comprehensive - know the audience and only include information that the audience need to know
- Technical documentation build on researching not plagiarism
## Don't write
- The job of technical writers are testers and researchers - increase personal knowledge (learning process), have selective information (none bias and accurate).
## Define the audience
- Don't assume anything about your audience while writing (always make sure have accurate information)
- Divide reader into 3 groups: user (just want to archive something with the application), administrators (setup and maintenance application), developers(extend application or interfaces with code)
## Basic fundamental
- Need to know what you write about, and why the audience want it (do your research on audience and topic)
- Have a proper guidance to your application that target on what individual need (have the good organization)
- Depend on each audience, the installation will be difference (consumer - short and easy to understand; sever application- long and details)
- Have an instructions that guide user from knowing nothing to something - have enough information to convince reader to learn something
- Always try to verify your contents
## Style
- Consistency in writing style
- Bias towards including headers, table, list, diagram and image - make the writing more approach and simpler to follow
- Use inline styles to offset important text
- Try not to use verbify to obscure nouns
- Make sure you have proper sentence
## Catalog of Diff
- Always record change to the product (update your documentation)
- Change logs should be terse, minimalist and eminently scale - Online documentation
## Build a Website
Should build and host a website instead of PDF
- PDF: downloaded on hardware, and can never update them
- static website: hosting contents on a website give you a power to fix inaccuracies and keep your content in sync
- HTML: barely better than PDF, unable to fix potential critical issue until the next software version ships
## Help other write
- Encourages people to contribute in your documentation
## Publish frequency
- Quick sanity check and a glance at build logs - building the finished product and ensure it 

# Specific
## Lightweight markup
- XML - base language (XHTML, DocBook, DITA): reduce people ability to contribute on your application
- Lightweight markup writing content is straightforward to learn, readable, and weight in 179 characters
- Popular editors:
  - Atom
  - Sublime
  - Text
  -  Notepad++
  -  Vim
### Markdown
  - The most famous markup language with cleanest syntax. However, have limited set of feature and no define standard
  - Flavours of Markdown:
    - Github Flavored
    - MultiMarkdown
    - Markdown extra
    - CommonMark
  - there some online tools for using markdown without downloading editors.
### reStructuredText
  - Come from Python community, has an actual, standard implementation, and many features. It is a all purpose language
  - Sphinx - use for RST
### ASCII doc
  - popular in Linux community, equivalent to DocBook
### Latex
  - Have complex syntax and need a learning curve

## Using distributed Version control
- Git and Mercurial over centralized system
- DVC allow offline work, and superior for concurrent work on the same file
- For Github:
  - documentation and code branches stay in sync
  - easy for developers to contribute
- README file
  - quick summary
  - instructions how to build documentation
  - instructions how to contribute

## Don't Duplicate
- Break the writing into bite-sized pieces (topics)
- Topics should build in the subject that your documentation want to delivery to users
- Don't store similar copies of the same documentation in a version control - hard to maintenance
- Use condition text - selectively include and exclude file

## Make static website
- Can host static website on local computer without installing anything and compress and ship them with software application.
- basic step: provide static site generator with content (Lightweight markup) and theme (template HTML and CSS)
- static generators exist
  - Sphinx
    - specific build for documentation
    - feature javascript - based search out of box
  - Jekyll
  - Hugo
  - ASCII doc
  - Middleman
  - Metalsmith
  - MkDoc
  - Hexo
- Make time to custome the theme
- Github wiki - collection of Lightweight markup file, which help build the static website

## Rsync
- copy new version site onto older version site result in removed or renamed file not being overwritten and persisting on the server, solution is delete old site before copy
- Transfers only the file that need to be modified (use to keep staging and production servers in well sync)
- Github Pages use remote repository and push the finish site to it

## Metric
- A pointer to the correct course of action (valuable check against writer's thought and institution)
- Might reveal a major flaw, a minor tweak or a reasonable explanation that require no change
- **This is one of reason why hosting a static website is a better choice**
- In documentation, any solution should include mix of metrics (bug number, reader feedback, etc)

## Script your complexity Away
- publishing pipeline - steps through markup file become print ready documentation
- Pandoc - tool to convert between markup format

## Localization
- Localization: the process of translating documentation to other language - it hard to publishing often, lead to lower quality of documentation
- Easier to publish in single language
