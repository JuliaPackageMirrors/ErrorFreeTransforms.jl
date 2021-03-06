# ErrorFreeTransforms

[![Build Status](https://travis-ci.org/dsiem/ErrorFreeTransforms.jl.svg?branch=master)](https://travis-ci.org/dsiem/ErrorFreeTransforms.jl)
[![Coverage Status](https://img.shields.io/coveralls/dsiem/ErrorFreeTransforms.jl.svg)](https://coveralls.io/r/dsiem/ErrorFreeTransforms.jl)

Rounding errors are a common problem in floating point arithmetic. For a pair of
floating point numbers `a`, `b`, an error-free transformation (EFT) is an
operation that maps `(a, b)` into `(x, y)`, where `a ○ b = x + y` and `x = fl(a
○ b)` with `○` being either addition, subtraction or multiplication. Standard
EFTs are the `TwoSum` algorithm by Knuth (implemented as `err_add`) and the
`TwoProd` algorithm by Dekker (implemented as `err_mul`).

This package implements several EFTs from the scientific literature.


## Current status

This project is still very much a work in progress. It requires a recent build
of Julia 0.4 to work.
