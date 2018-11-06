---
layout: default
title: Projects
---

## Floem

[Floem](http://github.com/mangpo/floem) is a language, compiler, and runtime for programming NIC-accelerated applications. Floem enables offload design exploration by providing programming abstractions to assign computation to hardware resources; control mapping of logical queues to physical queues; access fields of a packet and its metadata without manually marshaling a packet; use a NIC to memoize expensive computation; and interface with an external application. The compiler infers which data must be transferred between the CPU and NIC and generates a complete cache implementation, while the runtime transparently optimizes DMA throughput. 

## GreenThumb

[GreenThumb](http://pl.eecs.berkeley.edu/projects/greenthumb/) is a framework for building superoptimizers. It is designed to be easily extended to a new target ISA. The framework provides an efficient cooperative search strategy that runs multiple search instances cooperatively. Each search instance employs either a symbolic, stochastic, or enumerative search. We develop an new enumerative search technique, called LENS, that rapidly prunes away invalid candidate programs by applying selective refinement and bidirectional search.

## Chlorophyll

[Chlorophyll](http://pl.eecs.berkeley.edu/projects/chlorophyll/) is a synthesis-aided compiler for unusual spatial architectures. The primary goal of the project is to provide a new way of building compilers for radical architectures with low-effort while its generated code is still efficient. Currently, Chlorophyll can generate code for GreenArrays chip, our stress case study.
The compiler uses constraint solving to partition a program to fit in many tiny cores, and applies superoptimization to automatically discover assembly-level optimizations.

### Demos

- Compiled gesture recognition application running on GreenArrays powered by a potato! ([video](http://youtu.be/6_JV7BlnBwo))
- Lemonade-bleach powered GreenArrays running our synthesized program ([video](http://youtu.be/zMfdef-nYGY))

## PataBricks

Extended [PetaBricks](http://projects.csail.mit.edu/petabricks) to automatically generate OpenCL kernels and present heterogeneity choices to the autotuner. Introduced hybrid CPU-work-stealing and GPU-work-pushing runtime system.