---
permalink: /projects/ml4collider.html
layout: project
title: ML4Collider
shortname: ml4collider
description: Machine Learning for Particle Physics in Colliders
website: 
team:
  - Pierre-Baldi
  - schsu
  - danielwhiteson
awards:
  - type: ARO
    number: 76649-CS 
  - type: NSF
    number: NRT-1633631
  - type: DOE
    number: DE-SC0009920
  - type: DOE
    number: DE-SC0015971

---


The data collected by the Large Hadron Collider (LHC) experiments are vast in both the number of collisions and in
the complexity of each collision.
A central role of machine learning in LHC physics is to improve this data reduction,
reducing the relevant information contained in the low-level, high-dimensional data into a
higher-level and smaller-dimensional space.
This project enables collaboration between particle physicists and computer scientists to aid in scientific discoveries using state-of-the-art machine learning methods for particle physics in colliders. We have several projects on the boundary of particle physics and machine learning:

- **Symmetry-embedded networks:** 
    - Symmetry Preserving Attention Networks (SPA-Net): A novel approach to jet-parton assignment, based on tensor neural networks using a generalized attention mechanism. Building networks whose internal symmetries mirror the symmetries of the data can result in dramatic improvements in performance [arXiv:2010.09206](https://arxiv.org/abs/2010.09206)
- **Machine Teaching, Physicists Learning:** 
    - An new approach to translating black-box networks into a small set of interpretable observables. As a demonstration, we apply our approach to the benchmark task of jet classification [arXiv:2010.11998](https://arxiv.org/abs/2010.11998)
     and electron identification [arXiv:2011.01984](http://arxiv.org/abs/2011.01984) in collider physics.
- **Fast Machine Learning:** 
    - Sparse AutoRegressive Model (SARM): An alternative to Generative Adversarial Networks (GANs), which explicitly learns the sparseness of the data with a tractable likelihood, making it more stable and interpretable than other methods. [arXiv:2009.14017](https://arxiv.org/abs/2009.14017)
    - Optimal Transport based Unfolding and Simulation (OTUS): An alternative approach to fast simulation, which can be trained directly from data in an unsupervised manner, with the potential to replace full simulation rather than augment it. IML seminar [slide](https://indico.cern.ch/event/852553/contributions/4059046/attachments/2128576/3584162/Howard_Jessica_4thIML2020SlidesFinal.pdf).

The new tools will be developed as open source codes to transform the nature of data analysis in colliders and maximize significant impact on particle physics.


