---
title: Example
author:
    - Andreas Schneider
    - Example Author 2
    - Example Author 3
date: 2016
...

<!-- Simple control ofer placement of "Table of ..." -->
# {.frontmatter}
# {.toc}
# {.tot}
# {.tof}

# {.bodymatter}

# Introduction

This document is a simple example to demonstrate some of the features
of my pandoc-xhtml branch.

Compilation using requires at least the pandoc parameters: `-S --html-q-tags --section-divs -t html`.
For a more complete example look at the accompanying `Makefile`.

# Extensions

## Floats

Here is a simple example to get a floating table (with caption). This [Table](#tbl:test) can also be referenced.

+--------------+-----------+------------+
|   Column1    |  Column2  |  Column3   |
+==============+===========+============+
| Some content | more      | even more. |
+--------------+-----------+------------+
| Another line | with more | content.   |
+--------------+-----------+------------+

: <float id="tbl:test" options="here,force"/> Test table

Images work too:

![Some Image](image1){#img:example options="height=2cm"}

## Math

Math can be rendered TeX compatible when `--gladtex` is passed to pandoc. Then you can have nice little equations like $x^5 + \frac{4}{5}$.

## Symbols

You can use <span class="tex-logo">ConTeXt</span>-supplied symbol sets. For example you will see an envelope here: <span class="symbol" set="martinvogel 2">Letter</span>.

(If your chosen font supports the full or at least necesary set of symbols, you might as well just use the unicode symbols directly.)