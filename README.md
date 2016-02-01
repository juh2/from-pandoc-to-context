# pandoc-xhtml

`pandoc-xhtml.tex` offers a way to compile _Markdown_ documents with ConTeXt.

`pandoc-xhtml.tex` is an environment, which is what ConTeXt needs to compile XML sources directly.

With the proper environment, ConTeXt deals with XML natively. It doesn't need any intermediate format. Not even a ConTeXt source file cotaining the text to be typeset.

## What Is Wrong with ConTeXt Sources?

`pandoc` can generate ConTeXt documents from _Markdown_ sources. But this way you'll miss:

* Main document language information.

* Markup for language in text portions.

* Any `<div>` or `<span>` elements markup.

Generating the PDF document from XML sources with ConTeXt avoids loosing relevant information (such as language, which result in wrong hyphenation) or special layout for block or inline elements.

Going this way, the _Markdown_ source document may fulfill the promise:

> One source to generate them all.

## Status

This project is still work in progress. It is forked from https://github.com/ousia/from-pandoc-to-context, which provides a great basis but lacks a few features I need for my work.

### Extensions

The following features were added to the original version:
* Separate Table of Contents, Figures and Tables (TOC, TOF and TOT)
* Tables
* Images
* (Fixes wherever applicable)

## License

The environment file from this project (`pandoc-xhtml.tex`) is licensed to the public under the GNU General Public License; either [version 2](https://www.gnu.org/licenses/gpl-2.0.html), or (at your option) any [later version](https://www.gnu.org/licenses/gpl.html).

## Acknowledgments

This work was based on the extraordinary achievements of John MacFarlane (Pandoc) and Hans Hagen (ConTeXt) as well of course as Pablo Rodríguez (the base implementation of pandoc-xhtml).