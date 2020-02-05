# CUDA MeanShift
### A simple implementation of MeanShift algorithm with CUDA.

In this repo the parallel version of Mean Shift algorithm is presented; this repo belongs to the Master Degree Parallel Computing course project at UNIFI; here the link to its [sequential version](https://github.com/pisalore/MeanShift_sequentialCPP). Here the related [paper](https://github.com/pisalore/MeanShift_CUDA/blob/master.

## Getting Started

For parallel Mean Shift algoithm implementation I used CUDA with Windows 10. In particular:
* [Visual Studio 2019](https://visualstudio.microsoft.com/it/vs/)
* [CUDA 10.2](https://developer.nvidia.com/cuda-downloads)
* [Thrust LIbrary](https://docs.nvidia.com/cuda/thrust/index.html)

I strictly reccomend to read the [CUDA installation Guide](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html).
A very common problem is linked to the VS2019 Linker using CUDA, and dependencies: under Project Properties > Linker > Input > Additional Dependencies remember to copy: **cudart_static.lib;kernel32.lib;user32.lib;gdi32.lib;winspool.lib;comdlg32.lib;advapi32.lib;shell32.lib;ole32.lib;oleaut32.lib;uuid.lib;odbc32.lib;odbccp32.lib;%(AdditionalDependencies)** in order to correctly link cuda library.
Debug has to be x64 based.

<img src="https://github.com/pisalore/MeanShift_CUDA/blob/master/ms_2d_bw_2.gif" width="600" height="400">




