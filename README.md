# OpenCL Tutorials

## Requirements

The presented tutorials were developed and tested on Windows 10, Visual Studio 2019 and [Intel SDK for OpenCL](https://software.intel.com/en-us/intel-opencl) so that can be run on Windows PCs in the computing labs. Tutorial 4 also depends on the Boost library. If you would like to develop your OpenCL programs on your computer you have two options:
 - replicate the [Windows setup](#Windows-Setup) from the computing labs;
 - use the [multi_os](https://github.com/gcielniak/OpenCL-Tutorials/tree/multi_os) branch, which should allow to run the tutorials on different operating systems, programming environments and OpenCL SDKs. There is limited documentation for this option, however, so you should choose that option if you are comfortable with a CMake tool.
 
## Windows Setup
 - Windows 10, Visual Studio 2019
 - install [Intel SDK for OpenCL](https://software.intel.com/en-us/intel-opencl)
 - install OpenCL runtime drivers so that you can run the tutorials on different computing hardware installed on your computer. This step is hardware/vendor specific so you should find runtime drivers for your particular device on th eamnufacturer's website (e.g. [Intel CPUs](https://software.intel.com/en-us/articles/opencl-drivers), for NVIDIA GPUs these are included together with the recent graphics driver).
 - install the recent [Boost library Windows binaries](https://sourceforge.net/projects/boost/files/boost-binaries/) (e.g. VS2019 [boost_1_72_0](https://sourceforge.net/projects/boost/files/boost-binaries/1.72.0/boost_1_72_0-msvc-14.2-64.exe/download)). Then, add two environmental variables in the command line specifying the location of the include and lib Boost directories. For example, with boost_1_72_0 the commands would look as follows: `setx BOOST_INCLUDEDIR "C:\local\boost_1_72_0"` and `setx BOOST_LIBRARYDIR "C:\local\boost_1_72_0\lib64-msvc-14.2"`.
 - A useful reference if you are struggling to get it going: [OpenCL on Windows](http://streamcomputing.eu/blog/2015-03-16/how-to-install-opencl-on-windows/).
