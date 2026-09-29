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
    - label: "<i class='fas fa-file-alt'></i> Read the Paper (PRE)"
      url: "https://doi.org/10.1103/4dhv-8xd7"
    - label: "<i class='fas fa-scroll'></i> arXiv"
      url: "https://arxiv.org/abs/2602.24123"
    - label: "<i class='fab fa-gitlab'></i> GitLab Code"
      url: "https://gitlab.tudelft.nl/idema-group/mesomem"
  og_image: /assets/img/mesomem/fig3.png
  og_image_alt: "Overview of membrane systems simulated with MesoMem"

excerpt: >
  **MesoMem** — A mesoscale membrane model based on an additive potential.<br>
  <small>Pietro Sillano &nbsp;·&nbsp; Siewert J. Marrink &nbsp;·&nbsp; Timon Idema</small><br>
  <small><em>Physical Review E</em> <strong>114</strong>, 034412 (2026)</small>

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
      Bending rigidities in the biologically relevant range of 10–30 k<sub>B</sub>T and
      area compressibility moduli calibratable to experimental values.
  - title: "Rich Extensions"
    excerpt: >
      Supports **spontaneous curvature**, multiple lipid types, and adhesive interactions
      with colloidal nanoparticles. **Osmotic pressure** can be applied to vesicles by adding
      explicit solvent particles inside and outside, while the membrane model itself stays solvent-free.
---

{% include feature_row id="intro" type="center" %}

## Key Features

{% include feature_row %}

---

## Overview of Simulated Systems

<figure class="mesomem-figure">
  <img src="/assets/img/mesomem/fig3.png" alt="Overview of MesoMem simulated lipid systems">
  <figcaption>
    Overview of simulated lipid systems.
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

## Capabilities

{% include feature_row id="feature_row_physics" %}

---

## Tutorials

Step-by-step tutorials on planar membranes and vesicles are coming soon.

---

## Citation

If you use MesoMem in your research, please cite:

> P. Sillano, S. J. Marrink, and T. Idema, MesoMem: A mesoscale membrane model based on an additive potential, *Phys. Rev. E* **114**, 034412 (2026). [https://doi.org/10.1103/4dhv-8xd7](https://doi.org/10.1103/4dhv-8xd7)

```bibtex
@article{4dhv-8xd7,
  title = {MesoMem: A mesoscale membrane model based on an additive potential},
  author = {Sillano, Pietro and Marrink, Siewert J. and Idema, Timon},
  journal = {Phys. Rev. E},
  volume = {114},
  issue = {3},
  pages = {034412},
  numpages = {11},
  year = {2026},
  month = {Sep},
  publisher = {American Physical Society},
  doi = {10.1103/4dhv-8xd7},
  url = {https://link.aps.org/doi/10.1103/4dhv-8xd7}
}
```
