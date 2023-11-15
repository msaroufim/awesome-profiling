# Awesome profiling

## General utilites
* [https://ebpf.io/](https://ebpf.io/): Revolutionary sandboxed kernel profiling technology that makes it easier to build various profiling utilities. Tons of options here in Python https://github.com/iovisor/bcc
* [Dtrace](https://www.oracle.com/solaris/technologies/dtrace-tutorial.html): Available on Solaris (includes Mac but not Ubuntu) with notable highlights `prstat` and `mpstat`. `prstat` is not available on Ubuntu but can be replicated with `htop` and `ps`
* [collectl](http://collectl.sourceforge.net/Tutorial.html): Full system level profiling including CPU, disk, memory and network
* [perf](https://perf.wiki.kernel.org/index.php/Main_Page): CPU level performance counters
* [gprof](https://sourceware.org/binutils/docs/gprof/): sampling and instrumentation aware profiling
* [google perf tools](https://github.com/gperftools/gperftools)
* [Heaptrack](https://github.com/KDE/heaptrack): a heap memory profiler for linux
* [jemalloc](https://github.com/jemalloc/jemalloc): another heap memory profiler
* [ETW](https://docs.microsoft.com/en-us/windows-hardware/drivers/devtest/event-tracing-for-windows--etw-): Event tracing for windows
* [Mac OS instruments](https://knowledge.broadcom.com/external/article/180011/how-to-use-macintosh-xcodes-instruments.html): Mac OS instruments for profiling based on top of Dtrace
* [Renderdoc](https://github.com/baldurk/renderdoc): Multi platform graphics debugger for OpenGL and Vulkan
* [Windows Perf Analyzer](https://docs.microsoft.com/en-us/windows-hardware/test/wpt/windows-performance-analyzer): If `htop` could plot lines, windows only but recently added support for android
* [htop](https://htop.dev/): Visualize utilization as bar charts or line charts, issue commands to processes
* [Magic Trace](https://github.com/janestreet/magic-trace): High resolution programmable traces

## Continuous Profiling
* [parca](https://github.com/parca-dev/parca): Continuous profiling for analysis of CPU and memory usage, down to the line number and throughout time. Saving infrastructure cost, improving performance, and increasing reliability
* [parca-agent](https://github.com/parca-dev/parca-agent): eBPF-based always-on profiler auto-discovering targets in Kubernetes and systemd, zero code changes or restarts needed! Supports multiple languages: C/C++, Rust, Go, Python, Ruby, Java, etc.

## Python specific
* [viztracer](https://github.com/gaogaotiantian/viztracer)
* [psutil](https://github.com/giampaolo/psutil): Like htop but from within your python code
* [pyinstrument](https://github.com/joerick/pyinstrument):python call stack visualizer
* [pycallgraph](https://github.com/gak/pycallgraph): Visualize call stack as a graph (Maintenance mode)
* [py-spy](https://github.com/benfred/py-spy): Sampling profiler for Python
* [line profiler](https://github.com/pyutils/line_profiler): Line by line profiling
* [palanteer](https://github.com/dfeneyrou/palanteer): Fanciest UI, looks like something out of the matrix
* [yappi](https://github.com/sumerc/yappi/): multi threaded profiling
* [Pycharm profiler](https://www.jetbrains.com/help/pycharm/profiler.html): Built in profiler in Pycharm
* [TAU](https://www.cs.uoregon.edu/research/tau/home.php)
* [gprof2dot](https://github.com/jrfonseca/gprof2dot): Graphical call stack visualizer (Maintenance mode)
* [snakeviz](https://jiffyclub.github.io/snakeviz/): Visualize python cprofile data
* [scalene](https://github.com/plasma-umass/scalene): CPU and GPU based profiling with a web GUI
* [pprofile](https://github.com/vpelletier/pprofile): Very low overhead line profile
* [austin-python](https://github.com/P403n1x87/austin-python): Line-level very low overhead time & memory profiler with web & terminal UI

## Java specific
* [JProfiler](https://www.ej-technologies.com/products/jprofiler/overview.html): Java profiler for cpu, multithreading, graphical call stack visualizer
* [Java visual VM](https://visualvm.github.io/download.html): Bundled with JDK

## Mobile specific
* [iOS](https://developer.apple.com/library/archive/documentation/ToolsLanguages/Conceptual/Xcode_Overview/MeasuringPerformance.html): Instruments app in Xcode
* [Android](https://developer.android.com/studio/profile/android-profiler): Android Profiler in Android Studio

## C# specific
* [Unity profiler](https://docs.unity3d.com/Manual/Profiler.html): profiling tools specific for game development

## C++ specific
* [Tracy](https://github.com/wolfpld/tracy): Windows only but very comprehensive and helpful for game development
* [Callgrind](https://valgrind.org/docs/manual/cl-manual.html): Valgrind extension

## Web specific
* [Chrome profiler](https://developer.chrome.com/docs/devtools/evaluate-performance/): Support for throttling, emulating weak hardware,

## Machine Learning specific
* [Pytorch profiler](https://pytorch.org/blog/introducing-pytorch-profiler-the-new-and-improved-performance-tool/): Visual profiles of computations and data loading for PyTorch models, requires changes to code

## CPU specific
* [ARM profiling](https://developer.arm.com/tools-and-software/server-and-hpc/debug-and-profile/arm-forge/arm-map/python-profiling): ARM specific profiling tools, heavyweight UI
* [Intel Vtune](https://www.intel.com/content/www/us/en/develop/documentation/vtune-help/top/analyze-performance/code-profiling-scenarios/python-code-analysis.html)
* [Intel GPA](https://www.intel.com/content/www/us/en/developer/tools/graphics-performance-analyzers/overview.html): Intel Graphics performance analyzer

## GPU specific
* [pynvml](https://github.com/gpuopenanalytics/pynvml): Like `nvidia-smi` for your code with deeper level instrumentation
* [NVIDIA visual profiler](https://developer.nvidia.com/nvidia-visual-profiler)
* [NVIDIA tools](https://developer.nvidia.com/tools-overview)
* [GPU View](https://docs.microsoft.com/en-us/windows-hardware/drivers/display/using-gpuview#:~:text=GPUView%20(GPUView.exe)%20is,processing%20on%20the%20video%20hardware.): Windows specific GPU profiling

## Books
* [System Performance Enterprise and the Cloud](https://www.amazon.com/Systems-Performance-Enterprise-Brendan-Gregg/dp/0133390098)
* [BPF Performance tools](https://www.amazon.com/Performance-Tools-Addison-Wesley-Professional-Computing/dp/0136554822)

## Blogs
* [Flame Graphs](https://www.brendangregg.com/flamegraphs.html): flame graphs vs flame charts, off cpu profiling, icicle charts and more
* [Sampling vs Tracing](https://danluu.com/perf-tracing/): sampling based profilers are easier to use since they don't require any code change while instrumentation based profilers require code changes but are generally more informative
* [C++ performance tools](https://www.reddit.com/r/cpp/comments/7kurp6/comment/drhpyfh/?utm_source=share&utm_medium=web2x&context=3): reddit post with tons of links

## Talks
* [scalene talk](https://www.youtube.com/watch?v=5iEf-_7mM1k)
* [Why performance matters](https://www.youtube.com/watch?v=r-TLSBdHe1A&)
* [Common performance anti-patterns](https://www.youtube.com/watch?v=YY7yJHo0M5I)

## Understanding code structure
* [pyreverse](https://www.redshiftzero.com/pyreverse-uml/): Get python classes and then visualize with `graphviz`
* [pdb](https://stackoverflow.com/questions/4929251/how-to-step-through-python-code-to-help-debug-issues): Use step in functionality or line by line to understand how your code works
* [IntelliJ UML Class diagrams](https://www.jetbrains.com/help/idea/class-diagram.html)
