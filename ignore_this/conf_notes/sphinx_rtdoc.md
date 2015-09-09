#Intro to Sphinx & Read The Docs

-  [reStructuredText](http://docutils.sourceforge.net/rst.html)
-  [Sphinx](http://sphinx-doc.org/)

##Why write docs
-  It lets you save the state of your mind WHEN you're writing the code
-  Marketing from you to OTHER devs; makes it easier for people to USE your project
-  Makes your code better
    +  Design document helps you think out what you're trying to do
-  Improves your writing

##reStructuredText
-  a lightweight markup language; plain text
-  has semantic meaning (separates meaning/structure from presentation)
-  Markdown vs RST
    +  Markdown is NOT semantic, it's HTML shorthand
-  Whitespace sensitive; extensible, powerful
-  Directives
    -  main source of extensibility
    -  SPhinx builds on this
*  Inline markup
*  rst.ninjs.org

##Sphinx: Documentation generator
-  Great community & lots of prior art
-  additions it provides
    +  TOC tree
        *  allows hierarchical notation of documents
        *  gives an index page of all your content
    +  Cross-referencing
        *  ref content in other doc, Intersphinx across projects
    +  tons of code-specific markup
        *  Environment variables, RFCs, Tokens, Keywords, Classes, Filenames, Man pages
    +  Syntax Highlighting via Pygments
    +  Extensible
        *  ships w/ doctest runner, API for defining your own extensions
    +  Autodoc
        *  pulls docstrings out of your methods/functions/classes
        *  runs dynamically, to stay updated

##Read The Docs
-  Builds & hosts Sphinx docs
-  created at the 2010 Django Dash in 48 hours
-  Open Source