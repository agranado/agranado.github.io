---
title: "The Hidden Architecture of Cell Signaling"
date: 2024-01-15
draft: false
tags: ["signaling", "single-cell", "systems biology", "gene expression"]
description: "Discovering recurrent combinatorial patterns in how cells use signaling pathways"
---

Cell-cell signaling pathways—Wnt, Notch, TGF-β, Eph-ephrin—are the communication infrastructure of multicellular life. Each pathway comprises families of receptors that cells can express in different combinations. But which combinations actually occur in nature? And do different cell types use the same pathways in the same way?

These questions seem basic, but we didn't have answers. Until now.

## Mining Single-Cell Atlases

The explosion of single-cell RNA sequencing data created an opportunity. By integrating multiple public atlases, we could survey receptor expression across thousands of cell types from dozens of tissues.

The analysis wasn't trivial. Different datasets use different protocols, different annotations, different quality thresholds. I developed pipelines to harmonize this data and extract robust expression profiles for core signaling pathway components.

The result: **1,200+ combinatorial expression profiles** across major signaling pathways.

## Pathway Expression Motifs

The surprise was the structure we found.

You might expect receptor combinations to vary idiosyncratically—each cell type doing its own thing. Instead, we found **recurrent patterns**. The same receptor combinations appear again and again in unrelated cell types across different tissues and organs.

We called these recurring patterns "pathway expression motifs." Think of them as the vocabulary of signaling: a limited set of configurations that evolution has settled on, reused in different contexts.

Some motifs are restricted to related cell types (all epithelial cells use motif X). But others—the most interesting ones—appear in distantly related cells. A neuron and a fibroblast, separated by billions of years of evolutionary divergence, can use the same Wnt pathway configuration.

## Implications

This mosaic view of pathway usage has practical implications:

1. **Drug development**: If a signaling pathway operates in "modes," targeting the pathway might affect unexpected cell types that share that mode
2. **Development**: We found that motif usage is stable during aging but can change in punctuated transitions during development—suggesting these are true cell state markers
3. **Evolution**: The conservation of motifs suggests strong functional constraints on how pathways can be wired

## The Elowitz Lab Legacy

This work emerged from my postdoc with Michael Elowitz at Caltech, where I learned to ask "what is the space of possibilities?" before asking "why does biology do X?"

The signaling pathways themselves are ancient and well-studied. But the combinatorial space they occupy—the actual configurations that cells deploy—was uncharted. Mapping it required the single-cell data that only recently became available at scale.

**Publication**: Granados AA., Kanrar N., Elowitz MB. (2024). Combinatorial expression motifs in signaling pathways. *Cell Genomics* 4(1).
