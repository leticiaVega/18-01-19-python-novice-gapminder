---
title: "Running and Quitting"
teaching: 15
exercises: 0
questions:
- "How can I run python programs?"
objectives:
- "What is Python."
- "How to install python."
- "How to run and quit python."
keypoints:
- "Python programs are plain text files."
- "Use the Jupyter Notebook for editing and running Python."
- "The Notebook has Command and Edit modes."
- "Use the keyboard and mouse to select and edit cells."
- "The Notebook will turn Markdown into pretty-printed documentation."
- "Markdown does most of what HTML does."
---
## History
[Python][python]  was created in the early 1990s by Guido van Rossum at Stichting Mathematisch Centrum (see [CWI]) in the Netherlands as a successor of a language called ABC. Guido remains Python’s principal author, although it includes many contributions from others. Python was named for the BBC TV show Monty Python's Flying Circus.

## Some of Python's notable features.

*   Is an easy-to-use language that makes it simple to get your program working.
*   Runs anywhere, including Mac OS X, Windows, Linux, and Unix, with unofficial builds also available for Android and iOS.
*   Is free software in two senses. It doesn't cost anything to download or use Python, or to include it in your application. Python can also be freely modified and re-distributed, because while the language is copyrighted it's available under an open source license.
*   Uses an elegant syntax, making the programs you write easier to read.
*   Comes with a large standard library that supports many common programming tasks such as connecting to web servers, searching text with regular expressions, reading and modifying files.

## How to install python?

*   Download the most recent stable version. This is the one with the highest number that isn't marked as an alpha or beta release. Please see the [Python downloads][pythonDownload] page for the most up to date versions of Python 2 and Python 3.
*   In the case of Windows and Mac OS X, run the installer and accept the default installation location. Linux details will vary a bit depending on your Linux flavor.

## Python programs are plain text files.

*   They have the `.py` extension to let everyone (including the operating system) 
    know it is a Python program.
    *   This is convention, not a requirement.
*   It's common to write them using a text or code editor.
*   There are many around, and it is one of the most personal choices a programmer can make - Like a tennis-player choosing their racket. To start off with, you’ll just want a basic, easy-to-use one that doesn’t get in your way, but is still effective at writing python code. Here are some suggestions for those:

    *   [Gedit][geditEditor] and [Kate][kateEditor]: if you run Linux using Gnome or KDE respectively, you might already have one of these two installed!
    *   [Atom][atomEditor]: A new code editor available for Windows, Mac and Linux. It’s an open-source project developed by GitHub and is very easy to add functionality for, with its packages system.
    *   [Sublime Text][sublimeEditor]: A great all around editor that’s easy to use. It’s Ctl+B shortcut lets you run the python file you’re working on straight away. Runs on Windows, Mac and Linux.
    *   [NotePad++][notepadEditor]: A free source code editor and Notepad replacement that supports several languages. Running in the MS Windows environment, its use is governed by GPL License.

## Start python

*   Once you have installed Python, open a shell and type:

    ~~~
    $ python
    ~~~
    {: .python}

*   After Python opens, it will show you some contextual information similar to this:
    ~~~
    Python 3.6.3 |Anaconda custom (x86_64)| (default, Oct 27 2017, 12:14:30) 
    [GCC 4.2.1 Compatible Clang 4.0.1 (tags/RELEASE_401/final)] on darwin
    Type "help", "copyright", "credits" or "license" for more information.
    >>>
    ~~~
    {: .python}

   Note:
   The prompt `>>>` on the last line indicates that you are now in an interactive Python interpeter session, also called the “Python shell”. This is different from the normal terminal command prompt!

## Interacting with python

*   The python program that you have installed will by default act as something called an *interpreter*. An interpreter takes text commands and runs them as you enter them - very handy for trying things out.

*   You can now enter some code for python to run. Try:

    ~~~
    >>> 1
    1
    ~~~
    {: .python}

*   The interpreter acts as a simple calculator: you can type an expression at it and it will write the value. Expression syntax is straightforward: the operators +, -, * and / work just like in most other languages (for example, Pascal or C); parentheses (()) can be used for grouping. For example:

    ~~~
    >>> 2 + 2
    4
    >>> 50 - 5*6
    20
    >>> (50 - 5)*6
    270
    ~~~
    {: .python}

## Quitting python.

*   To leave the interactive shell and go back to the console (the system shell), press Ctrl-Z and then Enter on Windows, or Ctrl-D on OS X or Linux. Alternatively, you could also run the python command exit()!

    ~~~
    >>> exit()
    $
    ~~~
    {: .python}


## Markdown does most of what HTML does.

<div class="row">
  <div class="col-md-6" markdown="1">
~~~
*   Use asterisks
*   to create
*   bullet lists.
~~~
{: .python}
  </div>
  <div class="col-md-6" markdown="1">
*   Use asterisks
*   to create
*   bullet lists.
  </div>
</div>

<div class="row">
  <div class="col-md-6" markdown="1">
~~~
1.  Use numbers
1.  to create
1.  numbered lists.
~~~
{: .python}
  </div>
  <div class="col-md-6" markdown="1">
1.  Use numbers
1.  to create
1.  numbered lists.
  </div>
</div>

<div class="row">
  <div class="col-md-6" markdown="1">
~~~
*  You can use indents
	*  To create sublists 
	*  of the same type
*  Or sublists
	1. Of different
	1. types
~~~
{: .python}
  </div>
  <div class="col-md-6" markdown="1">
*  You can use indents
	*  To create sublists of the same type
*  Or sublists
	1. Of different
	1. types
  </div>
</div>

<div class="row">
  <div class="col-md-6" markdown="1">
~~~
# A Level-1 Heading
~~~
{: .python}
  </div>
  <div class="col-md-6" markdown="1">
# A Level-1 Heading
  </div>
</div>

<div class="row">
  <div class="col-md-6" markdown="1">
~~~
## A Level-2 Heading (etc.)
~~~
{: .python}
  </div>
  <div class="col-md-6" markdown="1">
## A Level-2 Heading (etc.)
  </div>
</div>

<div class="row">
  <div class="col-md-6" markdown="1">
~~~
Line breaks
don't matter.

But blank lines
create new paragraphs.
~~~
{: .python}
  </div>
  <div class="col-md-6" markdown="1">
Line breaks
don't matter.

But blank lines
create new paragraphs.
  </div>
</div>

<div class="row">
  <div class="col-md-6" markdown="1">
~~~
[Create links](http://software-carpentry.org) with `[...](...)`.
Or use [named links][data_carpentry].

[data_carpentry]: http://datacarpentry.org
~~~
{: .python}
  </div>
  <div class="col-md-6" markdown="1">
[Create links](http://software-carpentry.org) with `[...](...)`.
Or use [named links][data_carpentry].

[data_carpentry]: http://datacarpentry.org
  </div>
</div>

> ## Creating Lists in Markdown
>
> Create a nested list in a Markdown cell in a notebook that looks like this:
>
> 1.  Get funding.
> 2.  Do work.
>     *   Design experiment.
>     *   Collect data.
>     *   Analyze.
> 3.  Write up.
> 4.  Publish.
> 
> > ## Solution
> >
> > This challenge integrates both the numbered list and bullet list. 
> > Note that the bullet list is indented 2 spaces so that it is inline with the items of the numbered list.
> > ~~~
> > 1.  Get funding.
> > 2.  Do work.
> >     *   Design experiment.
> >     *   Collect data.
> >     *   Analyze.
> > 3.  Write up.
> > 4.  Publish.
> > ~~~
> > {: .python}
> {: .solution}
{: .challenge}

> ## More Math
>
> What is displayed when a Python cell in a notebook
> that contains several calculations is executed?
> For example, what happens when this cell is executed?
>
> ~~~
> 7 * 3
> 2 + 1
> ~~~
> {: .python}
> 
> > ## Solution
> >
> > Python returns the output of the last calculation.
> > ~~~
> > 3
> > ~~~
> > {: .python}
> {: .solution}
{: .challenge}

> ## Change an Existing Cell from Code to Markdown
>
> What happens if you write some Python in a code cell
> and then you switch it to a Markdown cell?
> For example,
> put the following in a code cell:
>
> ~~~
> x = 6 * 7 + 12
> print(x)
> ~~~
> {: .python}
>
> And then run it with shift+return to be sure that it works as a code cell.
> Now go back to the cell and use escape+M to switch the cell to Markdown
> and "run" it with shift+return.
> What happened and how might this be useful?
> 
> > ## Solution
> >
> > The Python code gets treated like markdown text.
> > The lines appear as if they are part of one contiguous paragraph.
> > This could be useful to temporarly turn on and off cells in notebooks that get used for multiple purposes. 
> > ~~~
> > x = 6 * 7 + 12 print(x)
> > ~~~
> > {: .python}
> {: .solution}
{: .challenge}

> ## Equations
>
> Standard Markdown (such as we're using for these notes) won't render equations,
> but the Notebook will.
> Create a new Markdown cell
> and enter the following:
>
> ~~~
> $\sum_{i=1}^{N} 2^{-i} \approx 1$
> ~~~
> {: .python}
>
> (It's probably easier to copy and paste.)
> What does it display?
> What do you think the underscore, `_`, circumflex, `^`, and dollar sign, `$`, do?
> 
> > ## Solution
> >
> > The notebook shows the equation as it would be rendered from latex equation syntax.
> > The dollar sign, `$`, is used to tell markdown that the text in between is a latex equation.
> > If you're not familiar with latex,  underscore, `_`, is used for subscripts and circumflex, `^`, is used for superscripts.
> > A pair of curly braces, `{` and `}`, is used to group text together so that the statement `i=1` becomes the the subscript and `N` becomes the superscript.
> > Similarly, `-i` is in curly braces to make the whole statement the superscript for `2`.
> > `\sum` and `\approx` are latex commands for "sum over" and "approximate" symbols. 
> {: .solution}
{: .challenge}

[anaconda]: https://docs.continuum.io/anaconda/install
[jupyter]: http://jupyter.org/
[markdown]: https://en.wikipedia.org/wiki/Markdown
[CWI]: https://www.cwi.nl/
[python]: https://www.python.org
[pythonDownload]: https://www.python.org/downloads/
[atomEditor]: https://atom.io
[sublimeEditor]: http://www.sublimetext.com
[geditEditor]: https://wiki.gnome.org/Apps/Gedit
[kateEditor]: https://kate-editor.org
[notepadEditor]: https://notepad-plus-plus.org
