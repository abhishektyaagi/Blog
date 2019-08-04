---
layout : default
---
### 1. SCALE-Sim: Systolic CNN	Accelerator Simulator[[Paper Link]](https://arxiv.org/abs/1811.02883)

- _STATED GOALS AND SOLUTIONS_

The authors are trying to tap into the dearth of simulators for developing DNN accelerators which provide a way to prototype ideas and analyze their performance. In the current work, they are considering only Systolic Array based accelerators as majority of the DNN accelerators are based on the Systolic Arraydesign.The authors provide us with a cycle-accurate systolic-array based CNN accelerator simulator, called SCALE-SIM. The authors have showcased the use-case of the said simulator by running applications from MLPerf benchmark and portraying the variation in performance, energy and scalability with different sizes of scratchpad memory, compute-array size etc.

- _SIGNIFICANT IDEAS_

This is probably the only simulation-emulation platform available out there when it comes to DNN accelerators. It exposes the various microarchitectural parameters to the user to study the interactions between them and the performance of the entire system. Moreover, unlike most of the works in this domain, SCALE-SIM takes into consideration the effects of integrating an accelerator with a simulator and how this is going to have an affect on the performance of the entire system.

- _FALLACIES AND BLIND SPOTS_

The paper talks about full-system integration with tools like Gem5, but hasn't been performed yet. Also, as the name suggests, the simulator is limited to the accelerators designed using systolic-array approach, which restricts the use-case for any other methodology. And lastly, the results obtained are by assuming that compute units are being utilized to the maximum utilization possible, which is difficult to achieve in the actual implementation. 

- _FUTURE WORK AND CONCLUSION_

With the complexity of system design increasing, I think integration with full-system simulators is necessary. Moreover, with functionalities like video captioning coming to handheld devices, there will be a need to accelerate networks other than CNN's (primarily LSTMs, LRCNs etc). Therefore, the work can be extended to incorporating the behavior of such networks on Systolic-Array based accelerators. Overall, I think it is a good step towards developing simulatio-emulation platforms for HW Accelerators design and will provide better understanding to how varying the different parameters at design time affects the final performance.

[back](/papers/papers_combine) 
