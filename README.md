# LIBSVMFileIO

Provides functions for reading and writing data files in the format used by
[LIBSVM](https://www.csie.ntu.edu.tw/~cjlin/libsvm/).


## Introduction
[LIBSVM](https://www.csie.ntu.edu.tw/~cjlin/libsvm/) has collected a number of
[data sets](https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/datasets/) in a
common format for benchmarking purposes. Easy acces to these publicly data sets
are useful even if one is not interested in using LIBSVM specifically. This a
bare-bones, stand-alone package whose only purpose is to read and write data to
files in the LIBSVM-format.

The package supports reading both classification and regression data as well as
multi-label data. The default behaviour is to load each data point as a sparse
vector. Partial loading where only a subset of the data points are loaded is
also supported.

## Usage
The package is currently not registered by can be intalled as any other package
by running the following in the Julia-REPL 
```julia
julia> using Pkg

julia> Pkg.add("<url to github>")
```

After insallation the package can be loaded like any other
```julia
julia> using LIBSVMFileIO
```

The package provides three functions `libsvmread`, `libsvmwrite`, and
`libsvmsize`. Documentation is provided via the inbuilt help functionallity. Run
any of
```julia
julia> ?libsvmread

julia> ?libsvmwrite

julia> ?libsvmsize
```
for more information.
