---
permalink: /projects/allen.html
layout: project
title: Algorithms for Allen
shortname: Allen
description: Extending the physics reach of LHCb by developing and deploying algorithms for a fully GPU-based first trigger stage
## website: https://ml-hep.org
team:
  - mdsokoloff
  - mityinzer
  - marianstahl
awards:
  - type: NSF
    number: OAC-2004364
  - type: NSF
    number: OAC-2004645
---

Data sets collected by  LHC experiments are some of the largest in the world. For example, 
the sensor arrays of the LHCb experiment produce about 100 terabytes per second 
and close to a zettabyte per year. 
Even after drastic data-reduction performed by custom-built 
read-out electronics, the data volume is still about 10 exabytes per year. 
Such large data sets cannot be stored indefinitely so all high energy physics (HEP) 
experiments employ a second data-reduction scheme executed in real time by a data-ingestion 
system -- referred to as a trigger system -- to decide whether each event is to be persisted for 
future analysis or permanently discarded. The primary goal of this project is developing and 
deploying software that will maximize the performance of the LHCb trigger system,
running its first processing stage on GPUs, so that the full physics discovery potential of LHCb is realized.

The LHCb detector is being upgraded for Run 3 
when the trigger system will need to process 25 exabytes per year. 
Currently, only 0.3 of the 10 exabytes per year processed by the trigger is analyzed using 
high-level computing algorithms; the rest is discarded prior to this stage using 
simple algorithms executed on FPGAs. 
To significantly extend its physics reach in Run 3, LHCb plans to process the entire 
25 exabytes each year using high-level computing algorithms. 
The entire first trigger-processing stage will be executed in GPUs using a custom-built framework called Allen.
The LHCb trigger makes heavy use of machine learning (ML) algorithms, which will need to be reoptimized 
both for Run 3 conditions but also for usage on GPUs. 

The specific objectives of this project are developing: GPU-based versions of the primary 
trigger-selection algorithms, which make heavy usage of ML; GPU-based calorimeter-clustering 
and electron-identification algorithms, likely using ML; 
and building the infrastructure required to deploy ML algorithms within the GPU-based trigger framework. 
These advances will make it possible to explore many potential explanations for dark matter, e.g., dark photon decays, 
and the matter/anti-matter asymmetry of our universe using data that would be 
otherwise inaccessible due to trigger-system limitations.

