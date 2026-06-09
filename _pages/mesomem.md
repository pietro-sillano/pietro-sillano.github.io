---
title: "MesoMem"
layout: splash
permalink: /mesomem/
author_profile: false
classes: wide

header:
  overlay_color: "#1a1a2e"
  overlay_filter: 0.6
  actions:
    - label: "<i class='fas fa-file-alt'></i> Read the Preprint"
      url: "https://arxiv.org/abs/2602.24123"
    - label: "<i class='fab fa-gitlab'></i> GitLab Code"
      url: "https://gitlab.tudelft.nl/idema-group/MesoMem"

excerpt: >
  **MesoMem** — A mesoscale membrane model based on an additive potential.<br>
  <small>Pietro Sillano &nbsp;·&nbsp; Siewert Jan Marrink &nbsp;·&nbsp; Timon Idema</small>

intro:
  - excerpt: >
      Bridging the gap between atomistic detail and continuum mechanics is a central challenge
      in modeling biological membranes, particularly for mesoscopic phenomena spanning large
      length and time scales. MesoMem is a solvent-free, one-particle-thick coarse-grained model
      for lipid bilayers governed by an **additive potential** that treats orientational elasticity
      through distinct tilt and splay energy terms. The model is implemented as a custom pair-style
      in the **LAMMPS** molecular dynamics engine and is freely available.

feature_row:
  - title: "Additive Potential"
    excerpt: >
      Orientational elasticity is split into independent **tilt** and **splay** energy terms,
      offering an unbiased potential form and direct physical interpretation of each contribution
      to membrane mechanics.
  - title: "Mesoscale Efficiency"
    excerpt: >
      Each particle represents a bilayer patch of ~300 lipids. The model accesses
      **microsecond timescales** and **micron-scale** membrane areas — far beyond what
      atomistic or standard coarse-grained models can reach.
  - title: "LAMMPS Implementation"
    excerpt: >
      Implemented as a custom pair-style in LAMMPS, with full support for MPI parallelization.
      The source code, example scripts, and tutorials are **openly available** on GitLab.

feature_row_physics:
  - title: "Self-Assembly & Vesiculation"
    excerpt: >
      Particles spontaneously assemble into lamellar structures and close into stable
      vesicles from a disordered state.
  - title: "Tunable Mechanics"
    excerpt: >
      Bending rigidities in the biologically relevant range of 10–30 k_BT and
      area compressibility moduli calibratable to experimental values.
  - title: "Rich Extensions"
    excerpt: >
      Supports **spontaneous curvature**, **osmotic pressure** via explicit solvent particles,
      multiple lipid types, and adhesive interactions with colloidal nanoparticles.
---

{% include feature_row id="intro" type="center" %}

## Key Features

{% include feature_row %}

---

## Overview of Simulated Systems

<figure style="text-align:center; margin: 2rem 0;">
  <img src="/assets/img/mesomem/fig3.png" alt="Overview of MesoMem simulated lipid systems" style="max-width:100%;">
  <figcaption style="margin-top:0.75rem; font-size:0.9em; color:#555;">
    <strong>Fig. 3</strong> — Overview of simulated lipid systems.
    (A) Self-assembled patches from 1500 randomly placed particles.
    (B) Planar membrane colored by <em>z</em>-height.
    (C) Vesicle with zero (red) and non-zero spontaneous curvature C₀ = 0.1 σ⁻¹ (blue) beads undergoing phase separation.
    (D) Spherical vesicle: cross-section (top) and full vesicle (bottom).
    (E) Membrane tube.
    (F) Cross-section of a vesicle wrapping a colloidal particle.
    (G) Planar membrane interacting with soft colloidal metaparticles.
  </figcaption>
</figure>

---

## Physics Covered

{% include feature_row id="feature_row_physics" %}

---

## Getting Started

Clone the repository and follow the build instructions to compile LAMMPS with the MesoMem pair-style:

```bash
git clone https://gitlab.tudelft.nl/idema-group/MesoMem
cd MesoMem
# See README for LAMMPS build instructions
```


Full example scripts are available in the [GitLab repository](https://gitlab.tudelft.nl/idema-group/MesoMem).

---

## Tutorials

- [Tutorial 1: Running a planar membrane](/mesomem/tutorial-1/)
- [Tutorial 2: Simulating a vesicle](/mesomem/tutorial-2/)

---

## Citation

```bibtex
@misc{sillano2026mesomem,
  title         = {MesoMem: A mesoscale membrane model based on an additive potential},
  author        = {Pietro Sillano and Siewert Jan Marrink and Timon Idema},
  year          = {2026},
  eprint        = {2602.24123},
  archivePrefix = {arXiv},
  primaryClass  = {cond-mat.soft},
  url           = {https://arxiv.org/abs/2602.24123}
}
```
