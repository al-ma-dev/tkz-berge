# Changelog — tkz-berge

All notable changes to `tkz-berge` are listed here, most recent first.

## [2.30c] — 2026/11/02

### Added
- Options `lua` and `3d` (or `3D`), as in tkz-graph: `\usepackage[3d]{tkz-berge}`.
  The documentation loads `tkz-berge` with the option `lua`.

### Examples
- New examples in `examples/latex` (PDF in `examples`): Kneser graph K(5,2),
  Ramsey R(3,3) = 6, Moser spindle, Mycielski's construction, de Bruijn
  graph B(2,3) (LuaLaTeX, `tkz-graph-lua`), Paley graph P13, Q4 as the
  lattice of subsets, Tower of Hanoi / Sierpinski graph S(4,3),
  Hoffman-Singleton graph, mystic rose K24, Coxeter graph.

### Documentation
- New section "New graphs and a gallery": `\grHypercube`, `\grTree` and
  the examples above.

## [2.20c] — 2026/10/20
### Changed
- Keys use the pgfkeys layer of tkz-graph instead of `xkeyval`: same names,
  same default values, same results.
- The macros call the internal commands of tkz-graph (`\tkzgr@Vertex`,
  `\tkzgr@Edge`, `\tkzgr@Edges`), not the short names.
- Needs tkz-graph 2.20c (2026-10-20) or later; an error is raised otherwise.
- `\grHypercube[options]{n}`: hypercube Q_n; vertices named by their binary
  word (`a000`, `a001`...); classic drawings for n = 1 to 4.
- `\grTree[options]{k}{depth}`: complete k-ary tree; vertex j of level l
  named `<prefix>l;j`.

### Examples
- NamedGraphs examples: each file has its own preamble (no more
  `\input{tkzpreamblenamed.ltx}`); `tkzNamed-12-2-0` loads `xcolor` with
  `dvipsnames`, `tkzNamed-15-2-0` declares its counter `tempi`.

## [2.00] — 2021/01/20
- Correction of bugs and new documentation.

## 1.00
- First version.
