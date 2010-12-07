#[Boost C++ Libraries](http://www.boost.org/)

This is a patched version of the [Boost C++ Libraries](http://www.boost.org/).
This should be the latest version (look at the _VERSION_ variable in the [build](boost/build) file).

Supported architectures are:

* armv7 (device)
* x86 (simulator)

Omitted libraries:

* python
* graph
* graph_parallel
* mpi
* wave
* program_options

The iostreams library is built, but without BZip2 compression support.

