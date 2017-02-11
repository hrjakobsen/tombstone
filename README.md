[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
# tombstone
tombstone.sty is a LaTeX package for drawing tombstone diagrams.

![Tombstone diagram example](https://cloud.githubusercontent.com/assets/3295293/22853815/e1ca4e5e-f05f-11e6-93b7-9b00e9dc7f9e.png)

## Installation
Simply copy the tombstone.sty file to the root directory of your projects and include it in your document using

```latex
\usepackage{tombstone}
```

## Example
The diagram in this readme was generated using the following code
```latex
\begin{tikzpicture}
    \begin{tombstonediagram}
        \compiler{cmp}{Java}{JVM}{JVM}{}
        \program[anchor=prg-2-2.north east]{prg}{Tetris}{Java}{at (cmp-1-1.north west)}
        \interpreter{int}{JVM}{x86}{at (cmp-2-2.south west)}
        \program{prgo}{Tetris}{JVM}{at (cmp-1-3.north east)}
        \machine{mac}{x86}{at (int-2-1.south west)}
    \end{tombstonediagram}
\end{tikzpicture}
```

## Documentation
The package is documented in the file tombstonedoc.tex. A compiled PDF version of the documentation is also included in the repository.
