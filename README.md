# Awesome profiling

## General utilites
* [https://ebpf.io/](https://ebpf.io/): Revolutionary sandboxed kernel profiling technology that makes it easier to build various profiling utilities. Tons of options here in Python https://github.com/iovisor/bcc
* [Dtrace](https://www.oracle.com/solaris/technologies/dtrace-tutorial.html): Available on Solaris (includes Mac but not Ubuntu) with notable highlights `prstat` and `mpstat`. `prstat` is not available on Ubuntu but can be replicated with `htop` and `ps`
* [collectl](http://collectl.sourceforge.net/Tutorial.html): Full system level profiling including CPU, disk, memory and network
* [perf](https://perf.wiki.kernel.org/index.php/Main_Page): CPU level performance counters
* [gprof](https://sourceware.org/binutils/docs/gprof/): sampling and instrumentation aware profiling
* [google perf tools](https://github.com/gperftools/gperftools)

## Python specific
* [psutil](https://github.com/giampaolo/psutil): Like htop but from within your python code
* [pyinstrument](https://github.com/joerick/pyinstrument):python call stack visualizer
* [pycallgraph](https://github.com/gak/pycallgraph): Visualize call stack as a graph (Maintenance mode)
* [py-spy](https://github.com/benfred/py-spy): Sampling profiler for Python
* [line profiler](https://github.com/pyutils/line_profiler): Line by line profiling
* [palanteer](https://github.com/dfeneyrou/palanteer): Fanciest UI, looks like something out of the matrix
* [yappi](https://github.com/sumerc/yappi/): multi threaded profiling
* [Pycharm profiler](https://www.jetbrains.com/help/pycharm/profiler.html): Built in profiler in Pycharm
* [ARM profiling](https://developer.arm.com/tools-and-software/server-and-hpc/debug-and-profile/arm-forge/arm-map/python-profiling): ARM specific profiling tools, heavyweight UI
* [Intel Vtune](https://www.intel.com/content/www/us/en/develop/documentation/vtune-help/top/analyze-performance/code-profiling-scenarios/python-code-analysis.html)
* [TAU](https://www.cs.uoregon.edu/research/tau/home.php)
* [gprof2dot](https://github.com/jrfonseca/gprof2dot): Graphical call stack visualizer (Maintenance mode)
* [snakeviz](https://jiffyclub.github.io/snakeviz/): Visualize python cprofile data

## Java specific
* [JProfiler](https://www.ej-technologies.com/products/jprofiler/overview.html): Java profiler for cpu, multithreading, graphical call stack visualizer

## C# specific
* [Unity profiler](https://docs.unity3d.com/Manual/Profiler.html): profiling tools specific for game development

## C++ specific
* [Tracy](https://github.com/wolfpld/tracy): Windows only but very comprehensive and helpful for game development
* [Callgrind](https://valgrind.org/docs/manual/cl-manual.html): Valgrind extension

## Machine Learning specific 
* [Pytorch profiler](https://pytorch.org/blog/introducing-pytorch-profiler-the-new-and-improved-performance-tool/): Visual profiles of computations and data loading for PyTorch models, requires changes to code
* [pynvml](https://github.com/gpuopenanalytics/pynvml): Like `nvidia-smi` for your code with deeper level instrumentation
* [NVIDIA visual profiler](https://developer.nvidia.com/nvidia-visual-profiler)

## Books
* [System Performance Enterprise and the Cloud](https://www.amazon.com/Systems-Performance-Enterprise-Brendan-Gregg/dp/0133390098)
* [BPF Performance tools](https://www.amazon.com/Performance-Tools-Addison-Wesley-Professional-Computing/dp/0136554822)

## Blogs
* [Flame Graphs](https://www.brendangregg.com/flamegraphs.html): flame graphs vs flame charts, off cpu profiling, icicle charts and more
* [Sampling vs Tracing](https://danluu.com/perf-tracing/): sampling based profilers are easier to use since they don't require any code change while instrumentation based profilers require code changes but are generally more informative
* [C++ performance tools](https://www.reddit.com/r/cpp/comments/7kurp6/comment/drhpyfh/?utm_source=share&utm_medium=web2x&context=3): reddit post with tons of links
