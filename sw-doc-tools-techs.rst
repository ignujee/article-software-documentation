============================================
Software Documentation: Tools and Techniques
============================================

- Markdown format Basics
- Restructured Text Basics
- Restructured Text Implementations
- md and rest Plugins for editers Emacs, vi, Atom, VSCode, Typora
- LynX and LibreOffice
- Python Docutils
- Pandoc for conversion from one format to another
- Third party Convertors for Restructured Text
- Sphinx: The Python Documentation Generator
- Documentation Hosting: GitLab and readthedocs.io


Markdown
========

Markdown is a text format documentation language which can be used to easily document software and systems
developed with the key design goal of readability. Modern editors like Vi, Atom, VScode and web based versioning systems like GitLab and GitHub support markdown. **Typora** is a markdown editor with live  preview. README.md file included in the source code of various free software
 is written in this lightweight markdown format. Emacs support for markdown can be enabled by installing the markdown-mode from MELPA.
The recommended way to install `markdown-mode` is to install the package from `MELPA` Stable using `package.el`. First, configure `package.el` and the MELPA Stable repository by adding the following to your `.emacs`, `init.el`, or equivalent startup file:

(require 'package)
(add-to-list 'package-archives
             '("melpa-stable" . "https://stable.melpa.org/packages/"))
(package-initialize)

Then, after restarting Emacs or evaluating the above statements, issue the following command: `M-x package-install RET markdown-mode RET`. When installed this way, the major modes markdown-mode and gfm-mode will be autoloaded and markdown-mode will be used for file names ending in either .md or .markdown

Markdown syntax
---------------

Using # we can create headings, eg #Welcome is equivalent to <h1>Welcome</h1> in HTML
Likewise we can create subheadings H2,H3 etc using ## and ### .
Alternatively  H1 and H2, can also be written as

`Heading1
`========

`Heading2
`--------

To create paragraphs, use a blank lines to separate one or more lines of text. Also make sure that you do not indent paragraphs with spaces or tabs.

To create a line break (<br>), end a line with two or more spaces, and then type return.

Giving emphasis to text can be done using *text* or _text_ for italics and **text** or __text__ for making a text in bold emphasis.

To get a text in bold italics embed the text with tree *'s or _. eg ___text___ or ***text***




