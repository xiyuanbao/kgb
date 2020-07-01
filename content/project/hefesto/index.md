---
title: HeFESTo
summary: Helmholtz Free Energy Self-consistent Thermodynamics
tags:
- HeFESTo
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Credit:Anna Matilde Lithgow-Bertelloni
  focal_point: Smart

links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
#url_code: ""
#url_pdf: ""
#url_slides: ""
#url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---

**Purpose**: Compute self-consistently the phase equilibria and equilibrium physical properties of sub-solidus mantle assemblages.

**Where to find**: https://github.com/stixrude/HeFESToRepository

**How to reference**: When using HeFESTo, please cite *Stixrude & Lithgow-Bertelloni* (2005) or *Stixrude & Lithgow-Bertelloni* (2011), depending on the application, and, if separate, the paper specifying the parameter set used. *Stixrude & Lithgow-Bertelloni* (2011) specifies the latest published parameter set (251010).

**Parameter sets and lookup tables**: Lookup tables for basalt, harzburgite and pyrolite using 251010 can be obtained by emailing either lstixrude@epss.ucla.edu or clb@epss.ucla.edu. *More coming soon!*

*Motivation*

This code grew out of an interest in the development of mineralogical Earth models and the exploration of the consequences and predictions of such models for other branches of geophysics. We felt that the large and rapidly growing base of knowledge on the nature of mantle phases and assemblages at high pressure had reached a state that construction of mineralogical Earth models seemed justified. Motivating questions include basic hypothesis tests: Are seismological observations of the mantle consistent with e.g. a lherzolitic composition? How do phase transformations and chemical heterogeneity interact in a convecting system? These have been central questions in the geophysics community for some time, and we felt that a general, flexible, self-consistent thermodynamics code would make a significant contribution towards answering them.

*Theory and capability*

The theory upon which the code is based has been described and illustrated with applications in previous publications [e.g. *Stixrude and Lithgow-Bertelloni*, 2005a, 2005b; *Xu et al*., 2008, *Stixrude and Lithgow-Bertelloni*, 2011; *Stixrude & Lithgow-Bertelloni*, 2012 ]. 

We have developed a thermodynamic formulation of mantle assemblages based on the concepts of fundamental thermodynamic relations and Legendre transforms and generalized to conditions of anisotropic stress and strain. For a given pressure, temperature, and bulk composition, the code computes the equilibrium phase assemblage (amounts and compositions of coexisting phases) the equilibrium physical properties of each phase and the assemblage, including but not limited to the density, heat capacity, enthalpy, thermal expansivity, bulk and shear moduli, and P- and S-wave velocities. The Voigt and Reuss bounds, and the Hill average of the moduli and velocities of the assemblage are computed.

*Significance for the geosciences community*

Two primary uses of this code would be: 1) As a component of a fully compressible convection code. The code can compute on an arbitrary pressure-temperature-composition grid, all thermodynamic quantities relevant to a convection calculation, including the density and enthalpy, including fully the influence of phase transformations. A lookup table based on the thermodynamics code would be a natural starting point for exploring the dynamics of realistic mantle mineralogical models. 2) Tests of hypothetical models of mantle composition against seismological observations. The crucial feature of our code that will permit central questions to be addressed more convincingly is the self-consistent treatment of phase equilibria and physical properties. To our knowledge, our code is the only one that accomplishes this along with the appropriate anisotropic generalization that is critical for comparison with seismology. 

*Benchmarks*

The code has been tested against a code widely used in shallow mantle and crustal applications: PERPLE_X by Connolly et al. (ETH) [e.g. *Connolly*, 2005]. In particular, Connolly independently reproduced our published phase diagram of a lherzolitic composition [*Stixrude and Lithgow-Bertelloni*, 2005a; *Stixrude and Lithgow-Bertelloni*, 2011].

*Cleaning up*

The code still needs documentation and optimization work. This is an ongoing effort.

*References*

Connolly J. A. D., Computation of phase equilibria by linear programming: a tool for geodynamic modeling and its application to subduction zone decarbonation, *Earth and Planetary Science Letters, 236*, 524–541, 2005.

Stixrude, L. and C. Lithgow-Bertelloni, Mineralogy and elasticity of the oceanic upper mantle: Origin of the low velocity zone, *Journal of Geophysical Research, 110*, B03204, 2005a, doi: 10.1029/2004JB002965.

Stixrude, L. and C. Lithgow-Bertelloni, Thermodynamics of mantle minerals: 1. Physical properties, *Geophysical Journal International*, *162*, 610-632, 2005b, doi: 10.1111/j.1365-246X.2005.02642.x.

W. Xu, C. Lithgow-Bertelloni, L. Stixrude and J. Ritsema, The effect of bulk composition on seismic structure, *Earth and Planetary Science Letters*, 275, 70-79, 2008, doi:10.1016/j.epsl.2008.08.012.

L. Stixrude and C. Lithgow-Bertelloni, Thermodynamics of mantle minerals II: Phase Equilibria*,* *Geophysical Journal International*, 184, 1180-1213, 2011, DOI: 10.1111/j.1365-246X.2010.04890.x

L. Stixrude and C. Lithgow-Bertelloni, Geophysics of chemical heterogeneity in the mantle*, Annual Reviews of Earth and Planetary Science*, 40, 565-595, 2012, 10.1146/annurev.earth.36.031207.124244.