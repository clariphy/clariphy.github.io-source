---
permalink: /projects/scailfin.html
layout: project
title: SCAILFIN
shortname: scailfin
description: Scalable CyberInfrastructure for Artificial Intelligence and Likelihood Free Inference (SCAILFIN)
website: https://github.com/scailfin
team:
  - mdhildreth
  - cranmer
  - heikomuller
  - msneubauer
  - danielskatz
awards:
  - type: NSF
    number: OAC-1841456
  - type: NSF
    number: OAC-1841471  
  - type: NSF
    number: OAC-1841448
---

The main goal of the SCAILFIN project is to deploy artificial intelligence and likelihood-free inference (LFI) techniques and software using scalable cyberinfrastructure (CI) to be integrated into existing CI elements, such as the [REANA system](https://www.reana.io/). Modular infrastructure has been constructed to support the running of extremely complex workflows on large HPC systems.  These workflows can orchestrate the generation of data for the training of complex ML algorithms at scale.

Current activities include the development of back-end modules for the REANA system that enable it to generate sequences of jobs on a variety of HPC systems, including CORI at NERSC and various XSEDE machines.  Various workflow languages are under investigation/implemention, including [PARSL](https://parsl-project.org/), [MLFlow](https://mlflow.org/), [CWL](https://www.commonwl.org/), and [Yadage](https://yadage.readthedocs.io/en/latest/).  The [MadMiner package](https://arxiv.org/abs/1907.10621) is in use to glue together the various aspects of the ML workflows. 
