# tkz-berge — tools for classic graphs of graph theory

Release 2.30c 2026/11/02

## Description

The package tkz-berge.sty is a collection of some useful macros if you want to
 draw some classic graphs of the graph theory or to make others graphs.
The macros are designed to give math  teachers (and students) easy access
at the programmation of drawing graphs with  TikZ.  I therefore hope that my
 packages provide  ideal tools for teachers wanting to offer their students fine documents of maths.

With LuaLaTeX, the options `lua` and `3d` of tkz-graph are also options of
tkz-berge: computations on the graphs (degrees, shortest path, coloring,
Eulerian paths...) and graphs in space with tkz-elements (prototype).
Without them the package is unchanged and works with pdfLaTeX.


## License

This work may be distributed and/or modified under the conditions of the
[LaTeX Project Public License](https://www.latex-project.org/lppl/), version 1.3c
or (at your option) any later version. See the files `LICENSE` and `lppl-1-3c.txt`.

This work has the LPPL maintenance status "maintained".
The Current Maintainer of this work is Alain Matthes.

## Requirements

The package compiles with utf8, pdflatex and lualatex, loads and depends on updated versions of:
- [tkz-graph](https://ctan.org/pkg/tkz-graph) 2.30c (2026/11/02) or later
- [tikz](https://ctan.org/pkg/tikz)

The options `lua` and `3d` need LuaLaTeX; `3d` also needs
[tkz-elements](https://ctan.org/pkg/tkz-elements) 6.10c (2026/11/01) or later.

## Installation

The package `tkz-berge` is present in TeXLive and MiKTeX, use the package
manager to install.

You can experiment with the `tkz-berge` and  `tkz-graph` packages by placing all of the
distribution files in the directory containing your current tex file.


## How to use it

To use the package `tkz-berge`, place the following line in the preamble of
your LaTeX document:

```
\usepackage{tkz-berge}
```
If you use the xcolor package, load that package before tkz-berge to avoid
 package conflicts.

\usepackage[usenames,dvipsnames]{xcolor}
\usepackage{tkz-berge}

With LuaLaTeX:

```
\usepackage[lua]{tkz-berge}   % computations on the graphs
\usepackage[3d]{tkz-berge}    % graphs in space (and computations)
```

## Documentation

The documentation is in english.
Documentation for `tkz-berge` is available on `CTAN`.

## Examples

All  examples given in documentation will be stored on `CTAN` as standalone
files, ready for compilation.

Other examples, in french, are on my site: [http://altermundus.fr](http://altermundus.fr)

## History

- 2.2 (2026/10/07) keys with `pgfkeys` (through tkz-graph 2.2) instead of
  `xkeyval`. Needs tkz-graph 2.2.
- 2.30c (2026/11/02) options `lua` and `3d` (LuaLaTeX), new examples and a
  gallery in the documentation (with `\grHypercube` and `\grTree`, added in
  2.20c). Needs tkz-graph 2.30c.

The full list of changes is in [CHANGELOG.md](CHANGELOG.md).

## Author

Alain Matthes, 5 rue de Valence, Paris 75005, al (dot) ma (at) mac (dot) com
