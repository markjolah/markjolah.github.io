---
layout: home
author_profile: true
title: About Me
---

I'm a computer scientist, mathematician and software engineer.  My research has previously focused on high-performance computational software for data processing, machine learning, statistical parameter inference, and stochastic simulation in scientific applications.

Currently I'm a software engineer at the [(JCSDA) Joint Center for Satellite Data Assimilation](https://www.jcsda.org/) working on the JEDI global weather model data assimilation project.  My research focuses on performance profiling and parallel algorithm development for MPI and OpenMP weather data assimilation on HPC resources.

 * [Publications](/publications/)
 * [Github projects list](/projects/)
 * [CV](/assets/pdf/MarkJOlah_CV.pdf)

---

# Featured Open Source Projects
## Mappel - **M**aximum **A** **P**osteriori **P**oint **E**mitter **L**ocalization
[![Mappel estimation objective](/assets/images/mappel_goal.png){:width="500px"}{:style="float: right;margin-right: 7px;margin-top: 7px;"}](/assets/images/mappel_goal.png)
[Mappel](https://markjolah.github.io/Mappel) is an object-oriented image processing library for [super-resolution localization](https://en.wikipedia.org/wiki/Super-resolution_microscopy#Localization_microscopy) of Gaussian point emitters in [fluorescence microscopy](https://en.wikipedia.org/wiki/Fluorescence_microscope#Sub-diffraction_techniques) applications.

 * [Mappel project site](https://markjolah.github.io/Mappel)
 * [Mappel github repository](https://github.co/markjolah/Mappel)

Point emitter localization is an essential image-processing sub-problem in many single-molecule microscopy applications.  Mappel can fit millions of emitter images in parallel in just a few seconds, making it orders of magnitude faster than other maximum-likelihood-based point estimation software.  Mappel achieves optimal estimation accuracy using robust, state-of-the art non-linear bounded optimization algorithms for maximum likelihood and maximum *a posteriori* estimation, as well as Markov-chain Monte Carlo posterior sampling for Bayesian inference.  These parameter estimation techniques allow Mappel to estimate confidence regions using [expected Fisher information](https://en.wikipedia.org/wiki/Fisher_information), [observed Fisher information](https://en.wikipedia.org/wiki/Observed_information), likelihood-ratio-based [profile likelihood intervals](https://en.wikipedia.org/wiki/Likelihood_function#Profile_likelihood), or with [Bayesian credible interval methods](https://en.wikipedia.org/wiki/Credible_interval).

Mappel is cross-platform (Linux/Win64) with object oriented interfaces for C++, Python, and Matlab, and GUI interfaces for interactive workflows and debugging.

<p align="center">
<a href="/assets/images/mappel_fitting_resolution.png" title="full size image"><img alt="Spdata GUI" src="/assets/images/mappel_fitting_resolution.png" width="400"/></a>
<a href="/assets/images/mappel_inspectorGUI.png" title="full size image"><img alt="Mappel maximizer inspector GUI" src="/assets/images/mappel_inspectorGUI.png" width="450"/></a>
</p>

## RPT - Robust Particle Tracker
[![RPT trajectories](/assets/images/rpt_tracks.png){:width="300px"}{:style="float: right;margin-right: 7px;margin-top: 7px;"}](/assets/images/rpt_tracks.png)
[RPT](https://github.com/markjolah/RPT) is a Matlab toolbox that provides a complete data processing toolchain for [single particle tracking](https://en.wikipedia.org/wiki/Single-particle_tracking) applications in [fluorescence microscopy](https://en.wikipedia.org/wiki/Fluorescence_microscope).  RPT is cross-platform (Linux/Win64) and consists of several components which are each implemented as parallel C++ libraries using OpenMP.  RPT is object-oriented, and allows for programmatic and GUI based, and batch-processing workflows.

Top-level RPT component software projects:
 * Emitter detection: [Boxxer](https://github.com/markjolah/Boxxer)
 * Localization: [Mappel](https://markjolah.github.io/Mappel)
 * Trajectory connection: [Tracker](https://markjolah.github.io/Tracker)

Publications using RPT software:
 * Samantha L. Schwartz, Cedric Cleyrat,  **Mark J. Olah**, Peter K. Relich, Genevieve K. Phillips, William S. Hlavacek, Keith A. Lidke, Bridget S. Wilson, and Diane S. Lidke. *Differential mast cell outcomes are sensitive to Fc&#949;RI-Syk binding kinetics*.  Molecular Biology of the Cell, 28(23). (2017)  [MBoC](https://www.molbiolcell.org/doi/full/10.1091/mbc.E17-06-0350) [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/28855374)


<p align="center">
<a href="/assets/images/rpt_spdata_gui.png" title="full size image"><img alt="Spdata GUI" src="/assets/images/rpt_spdata_gui.png" width="325"/></a>
<a href="/assets/images/rpt_gui.png" title="full size image"><img alt="RPT GUI" src="/assets/images/rpt_gui.png" width="325"/></a>
<a href="/assets/images/rpt_tsa.png" title="full size image"><img alt="RPT Trajectory Segment Analysis tools" src="/assets/images/rpt_tsa.png" width="275"/></a>

</p>

## MexIFace - Cross-platform C++ / Malab object-oriented MEX interface library and CMake build system
[![MexIFace structure](/assets/images/mexiface_diagram.png){:width="450px"}{:style="float: right;margin-right: 7px;margin-top: 7px;"}](/assets/images/mexiface_diagram.png)
The [MexIFace](https://markjolah.github.io/MexIFace) interface library provides a flexible means of wrapping a complex C++ library into a Matlab class via Matlab's MEX function extension method.  Ordinary Matlab C/C++ plugins are called *MEX* libraries and can only provide a simple function interface.

Interfaces using the [`MexIFace`](https://markjolah.github.io/MexIFace/classmexiface_1_1MexIFace.html) base class emulate a full object-based interface.  These hybrid C++/Matlab objects have Matlab methods and properties that affect state and perform computations in C++.

MexIFace is primarily designed to support high-performance numerical code, and uses the [Armadillo](http://arma.sourceforge.net/docs.html) matrix libraries to provide a computationally rich C++ object model while also allowing direct access to data stored in matlab array objects.  MexIFace supports OpenMP parallelization and linking of 64-bit integer versions of BLAS and LAPACK libraries as required by Matlab.
 * [MexIFace project site](https://markjolah.github.io/MexIFace)
 * [MexIFace github repository](https://github.com/markjolah/MexIFace#mexiface-)


## Tumble
**T**riangular **U**nstructured **M**esh with **B**ezier elements in a **L**agrangian **E**nvironment
![Tumble](/assets/images/tumble.png)

Tumble is a mesh geometry framework for representing fully [Lagrangian](https://en.wikiversity.org/wiki/Nonlinear_finite_elements/Lagrangian_and_Eulerian_descriptions) finite element simulations of [Navier-Stokes](https://en.wikipedia.org/wiki/Navier%E2%80%93Stokes_equations) fluid flow.  In a Lagrangian mesh, the elements move with the fluid they represent.  This causes elements to deform over time.  We handle this by using curved elements with [Bezier](https://en.wikipedia.org/wiki/B%C3%A9zier_curve) edges.  The *TUMBLE* package is responsible for moving the mesh elements, and running a sequence of cleaning phases to maintain mesh quality.  This includes flipping and re-interpolating elements to maintain the [Delaunay property](https://en.wikipedia.org/wiki/Delaunay_triangulation).

* Funded by the [Sangria Project](http://www.cs.cmu.edu/~sangria/) at Carnegie Mellon, which encompassed several computer science research groups targeting advanced parallel geometric and numerical algorithms and software for simulating complex flows with dynamic interfaces.
* [Tumble Project site](http://www.cs.cmu.edu/~sangria/tumble/index.html)
* [Tumble Documentation](http://www.cs.cmu.edu/~sangria/tumble/doc/index.html)
* Publications:
    * David E. Cardoze, Gary L. Miller, **Mark Olah**, Todd Phillips.  [*A Bezier-based moving mesh framework for simulation with elastic membranes.*](https://imr.sandia.gov/papers/abstracts/Ca314.html) Proceedings of the 13th International Meshing Roundtable. (2004) 71--79.


