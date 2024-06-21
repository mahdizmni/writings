---
title: "Test"
date: "2019-03-11"
description: "Sample article showcasing basic Markdown syntax and formatting for HTML elements."
tags: ["markdown", "css", "html", "themes"]
draft: false 
---

separator..5
separator
 MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest \
  MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest  MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest  MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest  MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest  MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest  MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest  MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest  MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest  MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest  MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest  MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest  MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest  MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest  MathJax
latest
Search docs
THE BASICS

What is MathJax?
MathJax Accessibility Features
Writing Mathematics for MathJax
The MathJax Community
Reporting Issues with MathJax
INCLUDING MATHJAX IN A WEB PAGE

Getting Started with Components
Configuring and Loading MathJax
The MathJax Components
Typesetting and Converting Math
Hosting Your Own Copy of MathJax
Making a Custom Build of MathJax
Examples in a Browser
MATHJAX ON A SERVER USING NODEJS

Getting Started with Node
Three Ways to Use MathJax in Node
Examples in Node
MATHJAX INPUT

TeX and LaTeX Support
Differences from Actual TeX
TeX and LaTeX math delimiters
TeX and LaTeX in HTML documents
Defining TeX macros
Automatic Equation Numbering
TeX and LaTeX extensions
The TeX/LaTeX Extension List
action
ams
amscd
autoload
bbox
boldsymbol
braket
bussproofs
cancel
cases
centernot
color
colortbl
colorv2
configmacros
empheq
enclose
extpfeil
gensymb
html
mathtools
mhchem
newcommand
newcommand Commands
noerrors
noundefined
physics
require
setoptions
tagformat
textcomp
textmacros
unicode
upgreek
verb
autobold
autoload-all
begingroup
mediawiki-texvc
Supported TeX/LaTeX commands
MathML Support
AsciiMath Support
MATHJAX OUTPUT

Output Formats
Lazy Typesetting
Line Breaking
Font Support
Browser Support
CONFIGURATION OPTIONS

Configuring MathJax
ADVANCED TOPICS

MathJax in Dynamic Content
Custom Extensions
The MathJax Processing Model
Synchronizing Your Code with MathJax
THE MATHJAX API

Using the MathJax API
MISCELLANEOUS

MathJax FAQ
MathJax Badges and Logo
Articles and Presentations
MATHJAX UPDATES

Upgrading from Version 2.x
What's New
 TeX and LaTeX Support The TeX/LaTeX Extension List newcommand Edit on GitHub
newcommand
The newcommand extension provides the \def, \newcommand, \renewcommand, \let, \newenvironment, and \renewenvironment macros for creating new macros and environments in TeX. For example,

\(
   \def\RR{{\bf R}}
   \def\bold#1{{\bf #1}}
\)
defines a macro \RR that produces a bold “R”, while \bold{math} typesets its argument using a bold font. See Defining TeX macros for more information.

This extension is already loaded in all the components that include the TeX input jax, other than input/tex-base. To load the newcommand extension explicitly (when using input/tex-base for example), add '[tex]/newcommand' to the load array of the loader block of your MathJax configuration, and add 'newcommand' to the packages array of the tex block.

window.MathJax = {
  loader: {load: ['[tex]/newcommand']},
  tex: {packages: {'[+]': ['newcommand']}}
};
Alternatively, use \require{newcommand} in a TeX expression to load it dynamically from within the math on the page, if the require package is loaded.

Since the nnewcommand extension is included in the combined components that contain the TeX input jax, it may already be in the package list. In that case, if you want to disable it, you can remove it:

window.MathJax = {
  tex: {packages: {'[-]': ['newcommand']}}
};
newcommand Commands
The newcommand extension implements the following macros: \def, \let, \newcommand, \newenvironment, \renewcommand, \renewenvironment

© Copyright 2021 The MathJax Consortium. Revision 1ac57add.

Built with Sphinx using a theme provided by Read the Docs.
 Read the Docsv: latest 