---
permalink: /projects/exatrkx.html
layout: project
title: Exa.TrkX
shortname: exatrkx
description: HEP Advanced Tracking Algorithms at the Exascale (Exa.TrkX)
website: https://exatrkx.github.io
team:
  - AdamAurisano
  - isobelojalvo
  - savvy379
  - p_calafiura
largeteam: true
awards:
  - type: DOE CompHEP
    number: DE-AC02-05CH11231
---

In the near future, the High Luminosity Large Hadron Collider (HL-LHC) at CERN and the Deep Underground Neutrino Experiment (DUNE) will come online.  In both cases, the expected physics programs are accompanied by new computational challenges in understanding the data.  The HL-LHC will run with a much higher collision rate than its predecessor, producing thousands of particles per beam crossing.  Reconstructing the trajectories of these particles is traditional performed using combinatorial search algorithms which scale poorly to these conditions.  Similarly, the DUNE detector will use liquid argon time projection chamber technology, which will provide millimeter-scale resolution 3D neutrino interaction imaging.  At these resolutions, track- and shower-like trajectories become challenging to distinguish.

Exa.TrkX, a DOE CompHEP project composed of physicists from the ATLAS, CMS, and DUNE experiments, is developing a collection of Graph Neural Network (GNN) models designed to improve particle reconstruction at next generation experiments with the speed necessary to cope with unprecedented data rates.  Rather than reconstruct trajectories sequentially, as is done traditionally, GNNs operate on graphs constructed from an event where the nodes represent measurements in a detector system and edges represent potential trajectories particles followed. After a series of message passing iterations, edges not corresponding to true trajectories are reduced in weight. To support the development of reconstruction techniques, Exa.TrkX is also pursuing distributed training of GNNs and their deployment on FPGA-based real-time processing systems.


