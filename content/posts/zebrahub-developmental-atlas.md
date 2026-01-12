---
title: "Zebrahub: Mapping Vertebrate Development One Cell at a Time"
date: 2024-11-15
draft: false
tags: ["single-cell", "developmental biology", "atlas", "zebrafish"]
description: "Building a multimodal atlas of zebrafish development with 500,000 cells"
---

How does a single fertilized egg become a complex organism with hundreds of distinct cell types? This question has driven developmental biology for over a century, but we've lacked the resolution to truly see the process unfold.

[Zebrahub](https://zebrahub.ds.czbiohub.org/) changes that.

## The Challenge

Zebrafish are a workhorse model organism—transparent embryos, rapid development, genetic tractability. But previous atlases captured snapshots: this cell type exists at this stage. What we wanted was a movie: how do cell states transition over time? Where are the decision points?

The challenge wasn't just scale (though 500,000 cells across development is substantial). It was integration: combining single-cell RNA-seq with imaging data, tracking lineages, and building a resource that researchers could actually use.

## What We Built

As lead computational biologist on the project, I developed the analysis pipelines that transformed raw sequencing data into biological insight:

- **Multimodal integration**: Aligning transcriptomic profiles with live imaging data to connect molecular states with physical cell behaviors
- **Trajectory inference**: Mapping the paths cells take as they differentiate, identifying branch points where fate decisions occur
- **State transition dynamics**: Characterizing the "late vertebrate pluripotent axial progenitors"—a transient population that gives rise to the body axis

The atlas is fully open-source and browsable at [zebrahub.ds.czbiohub.org](https://zebrahub.ds.czbiohub.org/).

## Key Findings

The most exciting discovery was about *how* cells make fate decisions. Rather than smooth, gradual transitions, we found punctuated changes—cells dwelling in metastable states before rapidly committing to a new identity.

This has implications beyond zebrafish. The mechanisms we identified are conserved across vertebrates. Understanding these dynamics could inform regenerative medicine, where we want to guide cells toward specific fates.

## The Bigger Picture

Zebrahub exemplifies what I love about computational biology: taking massive, heterogeneous datasets and extracting principles. The tools we built—for integration, visualization, trajectory analysis—are reusable. The biological insights are foundational.

This project also shaped how I think about building scientific resources. An atlas is only valuable if people use it. We invested heavily in the web interface, documentation, and making the data accessible to wet-lab biologists who may never write a line of code.

**Publication**: Lange M., Granados AA., et al. (2024). Zebrahub: Multimodal Zebrafish Developmental Atlas Reveals the State-Transition Dynamics of Late-Vertebrate Pluripotent Axial Progenitors. *Cell* 187(23).
