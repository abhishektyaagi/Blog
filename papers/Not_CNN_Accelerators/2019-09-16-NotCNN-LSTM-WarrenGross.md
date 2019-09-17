---
layout : default
---
### 1. Learning to Skip Ineffectual Recurrent Computations in LSTMs[[Paper Link]](https://arxiv.org/abs/1811.10396)

- _STATED GOALS AND SOLUTIONS_

The authors points out the presence of large number of ineffectual recurrent computations when it comes to LSTMs. They go on to explain how these computations can be skipped and can result in an increase in the performance which they showcase using a custom built accelerator that outperforms other state of the art accelerators for RNNs.

- _SIGNIFICANT IDEAS_

The work employs pruning on hidden-states values during the feed-forward phase of the computations to remove ineffectual computations. Moreover, the authors have carried out an analysis of the affects of sparsity on the prediction accuracy of the network to strike a right balance between advantages offered by ineffectual computations without loosing significant amount of prediction accuracy. At the hardware level, the authors do a good job of remembering the presence of zero values in the inputs across the time stamp without much of an overhead so as to ignore those computations in the coming timesteps

- _FALLACIES AND BLIND SPOTS_

For pruning the values, a threshold has been chosen by the authors but no discussion has been mentioned or cited related to reasoning behind selecting a particular threshold or how does the variation of threshold affects the prediction accuracy. The matrix-vector multiplication and Hadamard prodcut are calculated separately, but it is not clear if the delay between the two steps has been accounted in the final results.

- _FUTURE WORK AND CONCLUSION_

The paper has been very well compiled and is one of the very few works in its domain. It would be a nice exercise to try and understand the affect of different methods of quantization on the final accuracy. Considering all the talks about AutoML, I think it should be possible to explore the design space. Moreover, considering the reuse capability of weights across time steps, a scratchpad memory based design might bring more improvement in the power and performance numbers or similar exploration at the architectural level is required to give basis to a particular design selection.

[back](/papers/papers_combine)
