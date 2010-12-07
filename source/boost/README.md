#[Boost C++ Libraries](http://www.boost.org/)

This is a patched version of the [Boost C++ Libraries](http://www.boost.org/).
This should be the latest version (look at the _VERSION_ variable in the [build](boost/build) file).

###Supported architectures:

* armv7 (device)
* x86 (simulator)

###Omitted libraries

* python
* graph
* graph_parallel
* mpi
* wave
* program_options

###Issues

You must compile [bzip2](../bzip2) beforehand, or the iostreams library will produce an error:

    source/bzip2/build

