Breadcrumbs for LaTeX
=====================

Breadcrumbs for LaTeX documents

Introduces a pagestyle `breadcrumbs` that will print the current
'bread crumbs' of the document in the header.

No piece of text should be duplicated on the page; that is, if Section
B starts at some point on the page, Section B isn't printed in the
breadcrumb.  However, if content from Section A is visible on the same
page but the section header itself is not, Section A will appear in
the breadcrumb.

Licensed under the LaTeX Project Public License.

How It's Done
-------------

Programmed with LaTeX3, making essential use of sequences as stacks
(l3seq).  The stack is maintained throughout the document, pushing and
popping parts, chapters, sections, etc. for use elsewhere.

Since this stack is being maintained as pure data, its presentation is
a separate matter.  The main purpose of this package is to implement a
solution to http://tex.stackexchange.com/questions/122792/, so the
first exposition of the data I'll implement is through a header/footer
through the `fancyhdr` package.

---

Copyright 2013 Sean Allred

This work may be distributed and/or modified under the conditions of
the LaTeX Project Public License, either version 1.3 of this license
or (at your option) any later version.  The latest version of this
license is in http://www.latex-project.org/lppl.txt and version 1.3 or
later is part of all distributions of LaTeX version 2005/12/01 or
later.

This work has the LPPL maintenance status `maintained'.

The Current Maintainer of this work is M. Y. Name.

This work consists of the file brdcrmbs.sty.
