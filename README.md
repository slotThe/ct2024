# Pivotality, Twisted Centres, and the Anti-Double of a Hopf Monad

Source code for my [CT2024](https://www.usc.gal/regaca/ct2024/) poster.
[Here](https://tony-zorman.com/ct2024) is the accompanying website with the main references and additional notes.
A prebuild PDF of the poster is available [here](https://tony-zorman.com/posters/ct2024/poster.pdf).

## Cloning

As this project depends on submodules for its style file and poster class, cloning has to be done _recursively_.

``` console
$ git clone --recurse-submodules «URL»
```

If you have already cloned the repository, then submodules can be pulled in after the fact:

``` console
$ pwd
/home/«user»/poster-ct2024

$ git submodule update --init --recursive
```

## Building

Either `latexmk -pdf main` and hope for the best, or use the bundled flake:

``` console
$ nix build .?submodules=1
```
