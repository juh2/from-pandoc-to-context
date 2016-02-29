---
title: Example
author:
    - Andreas Schneider
    - Another Author
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

