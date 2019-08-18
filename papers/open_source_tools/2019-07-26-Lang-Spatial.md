---
layout : default
---
### 1. Spatial: A Language and Compiler for Application Accelerators [[Paper Link]](https://stanford-ppl.github.io/website/papers/pldi18_koeplinger.pdf)

- _STATED GOALS AND SOLUTIONS_

The aim of the paper is to come up with an efficient way of designing and programming Hardware Accelertors, along with carrying out designspace exploration to settle upon the best possible implementation for an application. To achieve the same, authors have presented Spatial, a new DSL and compiler framework which provides abstractions to program HW similar to HLS but offers control over key elements like Memory Hierarchy. It supports variety of platforms like FPGA, Reconfigurable HW (Plasticine) and C++ simulation  

- _SIGNIFICANT IDEAS_
... Machine Learning based design space exploration

This is probably the only simulation-emulation platform available out there when it comes to DNN accelerators. It exposes the various microarchitectural parameters to the user to study the interactions between them and the performance of the entire system. Moreover, unlike most of the works in this domain, SCALE-SIM takes into consideration the effects of integrating an accelerator with a simulator and how this is going to have an affect on the performance of the entire system.

- _FALLACIES AND BLIND SPOTS_

The paper talks about full-system integration with tools like Gem5, but hasn't been performed yet. Also, as the name suggests, the simulator is limited to the accelerators designed using systolic-array approach, which restricts the use-case for any other methodology. And lastly, the results obtained are by assuming that compute units are being utilized to the maximum utilization possible, which is difficult to achieve in the actual implementation. 

- _FUTURE WORK AND CONCLUSION_

With the complexity of system design increasing, I think integration with full-system simulators is necessary. Moreover, with functionalities like video captioning coming to handheld devices, there will be a need to accelerate networks other than CNN's (primarily LSTMs, LRCNs etc). Therefore, the work can be extended to incorporating the behavior of such networks on Systolic-Array based accelerators. Overall, I think it is a good step towards developing simulatio-emulation platforms for HW Accelerators design and will provide better understanding to how varying the different parameters at design time affects the final performance.

[back](/papers/papers_combine) 
