---
layout : default
---
### Aladdin: A Pre-RTL, Power-Performance Accelerator Simulator Enabling Large Design Space Exploration of Customized Architectures [[Paper Link]](https://www.eecs.harvard.edu/~shao/papers/shao2014-isca.pdf)

- _STATED GOALS AND SOLUTIONS_

The authors of the paper have presented a novel way of carrying out design space exploration of various architectural parameters when it comes to Custom Hardware Accelerator Design. To achieve this, the authors have presented an open-source toolset, Aladdin which is a pre-RTL power performance simulator which takes in high-level description of the algorithm as input and represents the accelerator using Dynamic Data Dependence Graphs(DDDG) where the nodes represent the operation and edges represents the dependencies. The authors have compared the performance of the said simulator against RTL based deisgn flow on benchmarks like GEMM, SHOC etc. 

- _SIGNIFICANT IDEAS_

Provides the flexibility of integrating it with full cache hierarchy models to explore the impact of memory hierarchy on accelerator performance. Comes with its own set of library for area and power analysis which gives it quick simulation speed without actually generating the RTL. And lastly, it models memory dependencies realistically by including memory ambiguation for input dependent memory accesses etc. 
- _FALLACIES AND BLIND SPOTS_

The simulator does not sweep across number of algorithms, rather targets different implementation of a particular algorithm. System calls, dynamic memory allocation in the input C-code are not modelled 

- _FUTURE WORK AND CONCLUSION_

Aladdin has been integrated with Gem5 to facilitate full system simulation and is available to be used in public domain. This work seems to take a step further than SCALE-Sim where it is not restricted to just Systolic-array baed accelerators. With it being available with Gem5, I think it puts it in front of simulatros like SCALE-Sim for simulation of HW Accelerator designs

[back](/papers/papers_combine) 
