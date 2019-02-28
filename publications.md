---
layout: single
author_profile: true
title: Publications
permalink: /publications/
---


## Single Particle Tracking with RPT
 * Samantha L. Schwartz, Cedric Cleyrat,  **Mark J. Olah**, Peter K. Relich, Genevieve K. Phillips, William S. Hlavacek, Keith A. Lidke, Bridget S. Wilson, and Diane S. Lidke. *Differential mast cell outcomes are sensitive to Fc&#949;RI-Syk binding kinetics*.  Molecular Biology of the Cell, 28(23). (2017)  [[MBoC]](https://www.molbiolcell.org/doi/full/10.1091/mbc.E17-06-0350) [[PubMed]](https://www.ncbi.nlm.nih.gov/pubmed/28855374)


 This paper used the [Mappel](https://markjolah.github.io/Mappel) project for accurately localizing point emitters at very low signal-to-noise ratios allowing us to use very low laser power so as to limit [photo-toxicity](https://www.microscopyu.com/references/cellular-phototoxicity) in very long single particle tracking experiments without sacrificing localization accuracy.  The [RPT](https://github.com/markjolah/RPT) package was used for single particle tracking.  We also used a custom Markov-chain Monte Carlo library to preform model selection and parameter inference for the lifetime analysis of single particle trajectories  that were best explained by a model with a mixture of geometric distributions.  See the Methods section for details on my contributions.

## Maximum likelihood estimation of Diffusion constant from noisy intermittent trajectories
 * Peter K. Relich, **Mark J. Olah**, Patrick J. Cutler, and Keith A. Lidke. *Estimation of the diffusion constant from intermittent trajectories with variable position uncertainties*. Physical Review E, 93. (2016) 042401. [[Phys. Rev. E]](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.93.042401) [[arXiv]](https://arxiv.org/abs/1508.02309)

 This paper describes the math behind the [DEstimator](https://markjolah.github.io/DEstimator) library, which provides a maximum-likelihood-based parameter estimator for accurately estimating the diffusion constant of particles from noisy intermittent observations.  Our method takes into account Gaussian noise in the observations convolved with the motion-blur effect inherent from the frame integration

<p align="center">
<img alt="DEstimator example trajectory" src="/assets/images/destimator_traj.png" width="200"/>
<img alt="DEstimator estimation accuracy" src="/assets/images/destimator_acc.png" width="350"/>
<img alt="DEstimator speed comparison" src="/assets/images/destimator_speed.png" width="450"/>
</p>

## Stochastic simulation of nano-scale molecular motors and chemical reactions.
 * **Mark J. Olah.** *Multivalent Random Walkers: A computational model of superdiffusive transport at the nanoscale*.  Ph.D. Dissertation.  University of New Mexico. (2012) [[PDF]](/assets/pdf/MarkJOlah2012-MultivalentRandomWalkers.pdf)
 * **Mark J. Olah** and Darko Stefanovic. *Superdiffusive transport by multivalent molecular walkers moving under load.* Physical Review E, 87. (2013) 062713. [[Phys Rev E]](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.87.062713) [[arXiv]](https://arxiv.org/abs/1211.3482)
* **Mark J. Olah** and Darko Stefanovic. *Multivalent random walkers: A model for deoxyribozyme walkers.* In *DNA Computing and Molecular Programming*, Vol.~6937 of *Lecture Notes in Computer Science*. Springer Berlin /Heidelberg. (2011) 160--174. [[Springer]](https://link.springer.com/chapter/10.1007%2F978-3-642-23638-9_14)

<p align="center">
<img alt="Molcular spider simulation experiment" src="/assets/images/spiders_experiment.png" width="800"/>
</p>

## Distributed data storage with object persistence using object-relational mapping
[![Natural entity state diagram](/assets/images/natent_states.png){:width="500px"}{:style="float: right;margin-right: 7px;margin-top: 7px;"}](/assets/images/natent_states.png)
 * **Mark J. Olah**, David Mohr, and Darko Stefanovic. *Representing uniqueness constraints in object-relational mapping: The Natural Entity framework.* In *Objects, Models, Components, Patterns*, volume 7304 of *Lecture Notes in Computer Science*. Springer Berlin / Heidelberg. (2012) 236--251.[[PDF]](https://pdfs.semanticscholar.org/10da/77d0ff57b4d266103f272c152b41fb92aba4.pdf)
<p align="center">
<a href="/assets/images/natent_speeds.png" title="full size image"><img alt="Distributed storage speeds for python numpy array accesses" src="/assets/images/natent_speeds.png" width="500"/></a>
</p>

## Stochastic modeling of super-diffusive and cooperative linear cargo transport with molecular motors
 * Oleg Semenov,  **Mark J. Olah**, and Darko Stefanovic. *Cooperative linear cargo transport with molecular spiders.* Natural Computing, 12(2). (2013) 259--276. [[Springer]](https://link.springer.com/article/10.1007%2Fs11047-012-9357-2)
 * Oleg Semenov, **Mark J. Olah**, and Darko Stefanovic. *Multiple molecular spiders with a single localized source---the one-dimensional case.* In *DNA Computing and Molecular Programming*, Vol.~6937 of *Lecture Notes in Computer Science*. Springer Berlin / Heidelberg. (2011) 204--216. [[Springer]](https://link.springer.com/chapter/10.1007/978-3-642-23638-9_17)
 * Oleg Semenov,  **Mark J. Olah**, and Darko Stefanovic. *Mechanism of diffusive transport in molecular spider models.* Physical Review E, 83. (2011) 021117. [[Phys Rev E.]](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.83.021117)

## Design of High-resolution cross reactive chemical sensor arrays using pattern recognition algoritms (SVM, KNN, PCA)
 * Renjun Pei, Aihua Shen, **Mark J. Olah**, Darko Stefanovic, Tilla Worgall and Milan N. Stojanovic. *High-resolution cross reactive array for alkaloids.* Chemical Communications, 22. (2009) 3193--3195. [[Chem. Comm.]](https://pubs.rsc.org/en/Content/ArticleLanding/2009/CC/b900001a)
 * Eric Green, **Mark J. Olah**, Tatiana Abramova, Lance R. Williams, Darko Stefanovic, Tilla Worgall, and Milan N. Stojanovic. *A rational approach to minimal high-resolution cross-reactive arrays*. Journal of the American Chemical Society, 128(47). (2006) 15278--15282. [[ACS]](https://pubs.acs.org/doi/abs/10.1021/ja0642663)

## Adaptive meshing algorithms for fully- Lagrangian finite element fluid dynamics simulations.
 * David E. Cardoze, Gary L. Miller, **Mark Olah**, Todd Phillips.  *A Bezier-based moving mesh framework for simulation with elastic membranes.* Proceedings of the 13th International Meshing Roundtable. (2004) 71--79. [[PDF]](https://imr.sandia.gov/papers/abstracts/Ca314.html)
