---
layout: default
---
### Glove Above [Team of 4]
[[Project Description]](https://2015.spaceappschallenge.org/project/glove-above/?fbclid=IwAR0Q6IObI59ZDQJ3bfFnOE8MOkF9HhEdFOR4d5fk0GUT8-iCenKiyt2kVkQ)[[Demo Video]](https://www.youtube.com/watch?v=pYe77UhBgKg)[[Source Code]]( https://drive.google.com/folderview?id=0B500nQ5c0n5OfnZTZUZLNlExRl85V3ZjcllhUzdpNDFGUlZYanNJcy1kbTIyQUhpNXg0UVU&usp=sharing)

The idea of Glove Above was born at the **2015 NASA Space App Challenege**, where we had to create an app/device in a two day hackathon at IIT-Delhi, which can have a purpose in outer space. The idea behind GLove Above was to help the astronauts have amazing recreational experiences in outer space to overcome monotony in a more intuitive way.It incorporates some critical features to deal with emergency and contingency situations. It recreates a fast and easy to use virtual keyboard, rich and intuitive experience of virtual musical instruments and a cool qualitative temperature sensing. 

- Runner's up, with a Global Nomination in **Spaceglove: Spacecraft Gesture And Voice Commanding** challenge category
- Awarded with **People's Choice Award**

### APOLLO: Compiler for automatic, dynamic and speculative parallelization and optimization of programs loop nests.[Team of 5]
[[Project Report]](https://drive.google.com/file/d/1PmaGCU59ezDTOep1gzAhRcYv9vmlTMtK/view)[[Demo Video(Credits: Juan Manuel Martinez Caamaño
)]](https://www.youtube.com/watch?v=zaM8va1SPw0)

The framework allows a user to mark in a C/C++ source code some nested loops of any kind in order to be handled by a speculative parallelization process, to take advantage of the underlying multi-core processor architecture. Loop nests whose memory accesses can be performed with pointers and indirections can be handled by Apollo.

Where conventional compiler rolls back to sequential operation on encountering non-linear memory accesses, APOLLO modells them as 'code bones' and can take advantage of the underlying multicore architecture for compiling such applications.

E
APOLLO's capabilities were tested against benchamrks like _SOR_ from the Scimark suite, _Backprop_ and _Needle_ from Rodinia Suite, _DMatmat_, _ISPMatmat_, _Spmatmat_ and _Pcg_ from the SPARK00 suite of irregular codes; and _Mri-q_ from the Parboil suite. The results of the comparisons on AMP Opetron 6172 and ARM Cortex A53 can be found [here](http://apollo.gforge.inria.fr/framework)

### Design of wireless interconnect based NoC for coherence support [Team of 2] 
[[Project Report]](https://drive.google.com/file/d/1UP46DG59cAHP1_eUuapubJl7F6CIuHfp/view)

We studied the advantages offered by Wireless Network on Chips and how they can be utilised to come up with a better cache coherence scheme for multi-core architectures

In a multi-core systems, the cores are clustered together on the basis of utilization of the cores. Each cluster possess a Wireless enabled core which can communicate with other clusters in a single-hop and hence therby reducing the latency associated with communication in larger multi-core systems.

The analysis of the abovementioned scheme is carried out at system level with the help of GEM5 simulation by running SPLASH2 and PARSEC benchmark. With the WiNoC, the architecture achieves a significant reduction(around 94%) in the L2 cache miss rate with a decrease in overall execution time as well.

### Power Performance improvement in MP SoC using Thread criticality prediction [Team of 2]

In multi-core systems various methods have been employed to predict critical-threads which are the bottleneck when it comes to overall processing of an application. 

We identified such threads with the help of their memory access pattersn where a weighted sum was calculated for their cache misses (higher weightage given to lower level of caches as data access time increases as we go down the memory hierarchy). Once the critical thread is identified, we employ DVFS technique to raise the Voltage and Frequency of that particular core so that it can be processed quicker. We also reduce the Voltage and Frequency of the other non-critical cores, to limit the overall power consumption within the limit.

The performance of this strategy was verified across four PARSEC benchmarks (Fluidanimate,Swaptions, Blackscholes, and Streamcluster) and an overall improvement of 15-20% was observed in the Energy-Delay Product (EDP).
