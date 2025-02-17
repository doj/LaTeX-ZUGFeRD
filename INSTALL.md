# Installation

## Recommended setup

As this package is now released via CTAN, it's highly recommended to use the TeX Live Manager (or the MikTeX console) for installation.

## Minimal portable TeX Live via DEPP

Additionally it's possible to use the Island of TeX's DEPP project to create a minimal portable TeX Live installation, only including the dependencies for this kind of documents.
This repository includes a `DEPENDS.txt` for this purpose.

Please be aware that the soft dependencies are those required to typeset the demo file.
In case you want to use a minimal setup for this the file `.tl_packages` contains all soft dependencies with a comment informing about the reason.

## Local user level installation using l3build

Additionally to the CTAN release this package includes an `l3build` installation script inside the package repository.
Details on usage can be found in the [l3build](https://github.com/latex3/l3build) [documentation](https://ctan.math.utah.edu/ctan/tex-archive/macros/latex/contrib/l3build/l3build.pdf).

To get started one can run:

```shell
l3build doc
```

within the repositories root directory.
This will build the Demo project as well as the current status of the documentation within the subdirectory `build/doc`.

To Install the package within your `$TEXMFHOME` there is also the `install` action:

```shell
l3build install
```

This will install the `zugferd.sty`  as well as the `zugferd-invoice.sty` and afterwards the TeX compiler will be able to find and use them.
