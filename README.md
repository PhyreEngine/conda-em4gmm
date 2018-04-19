This repository contains a [conda][conda] recipe for building [em4gmm][em4gmm],
a fast C implementation of the clustering expectation maximisation algorithm
for estimating Gaussian mixture models.

## Prerequisites

1. You will need an installation of [conda][miniconda].

2. Your root conda installation must have the `conda-build` installed.

## Building

You should be able to build this package by simply running `./build`.

## Patches

This recipe contains the following patches:

* `makefile.patch`
    Limits the number of threads used in testing, and allows `conda build`'s
    environment variables to pass through to the build commands.

[conda]: https://conda.io
[em4gmm]: https://github.com/juandavm/em4gmm
[miniconda]: https://conda.io/miniconda.html
