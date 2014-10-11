---
layout: default
title: Education
---

# Education
-----------

I graduated from **Indian Institute of Technology Kanpur** in 2010 with a B.Tech-M.Tech dual degree in Aerospace 
Engineering, with specialization in parallel numerical algorithms. My master's thesis was
titled *["Parallel Computation of 3-D Flow in a Mixed Compression Air-Intake"](downloads/thesis_rohit_saxena.pdf)*.

## Master's thesis
##### Dec 2008 - Jul 2010
#### Parallel Computation of 3-D Flow in a Mixed Compression Air-Intake.

- The objective was to study the behaviour of air-flow inside jet air-intakes at supersonic
  speeds by doing numerical simulations. The compressible nature of the flow and the presence 
  of shocks (discontinuity in media) makes its accurate simulation difficult.
- A Finite Element Formulation of the governing Navier-Stokes equations, a set of non-linear
  partial differential equations, was done to obtain a matrix system of linear equations. The
  solution to these equations gives the value of flow variables: velocity, pressure and tempreture,
  at discrete points in the domain.
- The size of the matrix system depends on the number of such discrete points in which the domain
  is divided and the degree of freedom of each point. This system needs to be solved for increasing 
  values of time to get a continuous solution in time. The size of the matrix system I was working on 
  was of the order of *10 million*. 
- To make this problem computationally tractable, it becomes necessary to solve it parallely, which was 
  the motivation for my thesis. I developed a solver in Fortran using **MPI** libraries, which partitions
  the domain into subdomains, and solves them on a multi-node cluster. Post processing routines were also
  developed to visualize the solutions obtained.
- The project was highly interdisciplinary involving concepts from Fluid Dynamics, Mathematics
  and Parallel Computing.


A copy of the thesis could be downloaded from [here](downloads/thesis_rohit_saxena.pdf).

I was also a **research assistant** for a couple of months in the CFD lab, during which I continued
work on the masters thesis.

- Scaled and did speed-up studies for the parallel application developed in my Master's thesis.
- Tweaked the application to adaptively determine the most optimal use of resources, memory
and processors, and allocate them dynamically based on speed-up analysis.

