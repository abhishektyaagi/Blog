---
layout : default
---
### 1. Spatial: A Language and Compiler for Application Accelerators [[Paper Link]](https://stanford-ppl.github.io/website/papers/pldi18_koeplinger.pdf)

- _STATED GOALS AND SOLUTIONS_

The aim of the paper is to come up with an efficient way of designing and programming Hardware Accelertors, along with carrying out designspace exploration to settle upon the best possible implementation for an application. To achieve the same, authors have presented Spatial, a new DSL and compiler framework which provides abstractions to program HW similar to HLS but offers control over key elements like Memory Hierarchy. It supports variety of platforms like FPGA, Reconfigurable HW (Plasticine) and C++ simulation

- _SIGNIFICANT IDEAS_

Spatial provides user with multiple abstractions to enable the right balance between productivity and performance oriented details. It provides multiple memory libraries which can be used to design the memory-hierarchy as per user requriement. Moreover, Spatial has the ability to statically analyse the memory access patterns to partition, buffer the memory space as per the application. Special host interface for communication. Makes use of active-learning based autotuner HyperMapper to keep the design space exploration points to a realistic level without considerable loss in accuracy.


- _FALLACIES AND BLIND SPOTS_

Programming and designing CGRAs has been restricted to Plasticine, but little has been written about programming other CGRAs with different architecture altogether. Productivity of the compiler has been measured with respect to the number of lines of codes which seems a bit crude way of analysing.

- _FUTURE WORK AND CONCLUSION_

In a gist, it seems to be a very unique tool in the domain of Hardware Accelerators with good community support and its utilizations has been succesful in some courses at Stanford. HyperMapper can be extended to spend less time on checking the validity of a design.

[back](/papers/papers_combine)
