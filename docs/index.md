# CJSaxton
---

## Recent Presentations:

### Spatially logarithmic simulations of Rayleigh-Bénard convection at high Ra
[Curtis&nbsp;J.&nbsp;Saxton](https://orcid.org/0000-0002-5441-1978),
[Keaton&nbsp;J.&nbsp;Burns](https://orcid.org/0000-0003-4761-4766),
[Rich&nbsp;R.&nbsp;Kerswell](https://orcid.org/0000-0001-5460-5337),
[Steven&nbsp;M.&nbsp;Tobias](https://orcid.org/0000-0003-0205-7716).

Turbulent convection at high Rayleigh numbers (Ra) involves active structures spanning orders of magnitude spatially,
in the bulk and in the boundary layers.
The required resolution can be expensive or impossible for direct numerical simulations (DNS).
We consider alternative schemes based on logarithmic grids in Fourier space.
Constant-coefficient linear operators are exact.
Nonlinear operators are approximated by finite lattice-supported triads
(somewhat akin to shell models, but enabling a range of nonlocal interactions).
We apply these lattices to horizontal dimensions,
combined with a Chebyshev representation vertically,
to investigate the scaling properties for the heat transport in Rayleigh-Benard convection up to extreme Ra.
As a side-effect of irrational k-space scaling,
the spatial domain is horizontally infinite (not a periodic box) and populated by asymmetric, nonrepetitive flow structures.
Thermal boundary layers are well resolved by the large Chebyshev resolution.
We discuss details of these emergent phenomena, and present the global scaling laws.
A few further methodological improvements could bring previously unattainable regimes into the reach of ordinary computer hardware.

2024-04-09,
[65th British Applied Mathematics Colloquium](https://conferences.ncl.ac.uk/bamc2024/),
Newcastle&nbsp;U., UK

---

### Entropy, complexity, and causality in direct and approximated fluid simulations
[Curtis&nbsp;J.&nbsp;Saxton](https://orcid.org/0000-0002-5441-1978),
[Ajay&nbsp;Chandrarajan&nbsp;Jayalekshmi](https://orcid.org/0000-0002-6447-581X),
[Anna&nbsp;Guseva](https://orcid.org/0000-0003-2831-184X),
[Ben&nbsp;F.&nbsp;McMillan](https://orcid.org/0000-0003-1509-2940),
[Steven&nbsp;M.&nbsp;Tobias](https://orcid.org/0000-0003-0205-7716)

Information entropy measures the disorder or inherent difficulty of predicting spatial and temporal structures
in a time-series or spatially in a high-dimensional dynamical system.
Statistical complexity characterises departures from equilibrium distributions (even given a fixed entropy),
and can distinguish deterministic from stochastic physics (chaos vs noise).
Related measures of causality quantify the relative influence of time-irreversible and 
-reversible processes (or directionality spatially).
Calculating these scores from direct numerical simulations can characterise the importance of coherent structures or turbulent transitions.
It is also interesting to compare the scores for physically equivalent models calculated via approximate methods
(e.g. generalised quasilinear models or data-driven codes).
The entropic cost of any approximation scheme is objectively derivable.
We consider diverse applications to
(e.g.) fluid thermal convection,
magneto-rotational turbulence,
and gyrokinetic plasma turbulence.

\[[PDF](20240125_saxton_poster.pdf)\]
2024-01-25/26,
[LIFD 5th Birthday Celebration](https://fluids.leeds.ac.uk/events/lifd-5th-birthday-celebration/),
U.&nbsp;Leeds, UK.

---

### Spatially logarithmic simulations of Rayleigh-Bénard convection
[Curtis&nbsp;J.&nbsp;Saxton](https://orcid.org/0000-0002-5441-1978),
[Keaton&nbsp;J.&nbsp;Burns](https://orcid.org/0000-0003-4761-4766),
[Steven&nbsp;M.&nbsp;Tobias](https://orcid.org/0000-0003-0205-7716),
[Rich&nbsp;R.&nbsp;Kerswell](https://orcid.org/0000-0001-5460-5337).

We investigate the heat transport and flow properties of 2D thermal convection
in a Boussinesq fluid at high effective resolution and extremes of convective driving (Rayleigh number). 
Upper and lower boundaries are isothermal,
with no-slip velocity conditions,
and the vertical grid is a Chebyshev array.
Horizontal modes evolve on a logarithmic grid in *k*-space,
with points at regular irrational intervals,
spanning >4 orders of magnitude spatially (at little computational cost).
Chosen lattice parameters affect the realism of spectra and energy transfers.
The domain is horizontally infinite,
and *x*-space snapshots can be rendered at any interval.
Freed from the implicit constraints of a standard periodic box,
non-repeating asymmetric flow structures can migrate.
Transient zonal flows are faster in some regimes.
Nusselt numbers (heat transfer) tend to follow a classical 1/3 power-law with Rayleigh numbers, even to high extremes.
This demonstration suggests that spatially
logarithmic simulations (on ordinary hardware)
can decisively resolve some physical models and conditions
that are computationally unaffordable using normal algorithms.

2024-01-11/12
[AMS80 Conference](https://conferences.ncl.ac.uk/ams80/), Newcastle&nbsp;U., UK

---

### Rotating thermal convection under generalised quasilinear approximations
[Curtis&nbsp;J.&nbsp;Saxton](https://orcid.org/0000-0002-5441-1978),
[J.&nbsp;Brad&nbsp;Marston](https://orcid.org/0000-0002-9751-829X),
[Jeffrey&nbsp;S.&nbsp;Oishi](https://orcid.org/0000-0001-8531-6570),
[Steven&nbsp;M.&nbsp;Tobias](https://orcid.org/0000-0003-0205-7716)

We model rotating Rayleigh–Bénard convection in 3D direct numerical simulations
of a periodic box with Boussinesq perturbations,
subject to inclined global rotation.
Vertical boundary temperatures are fixed locally, with a linear meridional gradient (T<sub>y</sub>).
We vary T<sub>y</sub> and convective driving.
Emergent flows can include thermal winds, anisotropic turbulence, and giant vortices.
Fully nonlinear (NL) runs provide benchmarks for testing quasilinear (QL) and general quasilinear (GQL) approximate dynamics.
In horizontal planes, each variable (*q*) splits into a Fourier “low” background (*q*<sub>L</sub>)
at \|*k<sub>x</sub>*\|,\|*k<sub>y</sub>*\|<*Λ*,
and a “high” variable for fluctuations (*q*<sub>H</sub>).
Varying the GQL cutoff (*Λ*=∞,10,5,1,0) selectively impairs spectral power transfers,
affecting flow morphologies, entropy, variability, local and global statistics.
Versions of GQL usually improve upon the accuracy of QL (*Λ*=0), but low-*Λ* can produce spurious inverse cascades.
Higher *Λ* improves realism more readily for models with stronger thermal winds.
GQL succeeds generally even in peculiar cases that never settle to one unimodal steady state.
Accuracy depends on the directness of boundary conditions, simple vertical profiles, 
and raising *Λ* to enclose the most active Fourier modes.
However, spatial anisotropies are *Λ*-sensitive in all our tests.

\[[DOI](http://dx.doi.org/10.13140/RG.2.2.13650.77764)\]
\[[PDF](20230911_saxton_poster1x.pdf)\]
2023-09-11 [GAFDEM](https://gafdem.sciencesconf.org/), Nice, France.

---

### Entropy, complexity, and causality in direct and approximated fluid simulations
[Curtis&nbsp;J.&nbsp;Saxton](https://orcid.org/0000-0002-5441-1978),
[Ajay&nbsp;Chandrarajan&nbsp;Jayalekshmi](https://orcid.org/0000-0002-6447-581X),
[Anna&nbsp;Guseva](https://orcid.org/0000-0003-2831-184X),
[Ben&nbsp;F.&nbsp;McMillan](https://orcid.org/0000-0003-1509-2940),
[Steven&nbsp;M.&nbsp;Tobias](https://orcid.org/0000-0003-0205-7716)

Information entropy measures the disorder or inherent difficulty of predicting spatial and temporal structures
in a time-series or spatially in a high-dimensional dynamical system.
Statistical complexity characterises departures from equilibrium distributions (even given a fixed entropy),
and can distinguish deterministic from stochastic physics (chaos vs noise).
Related measures of causality quantify the relative influence of time-irreversible and 
-reversible processes (or directionality spatially).
Calculating these scores from direct numerical simulations can characterise the importance of coherent structures or turbulent transitions.
It is also interesting to compare the scores for physically equivalent models calculated via approximate methods
(e.g. generalised quasilinear models or data-driven codes).
The entropic cost of any approximation scheme is objectively derivable.
We consider diverse applications to
(e.g.) fluid thermal convection,
magneto-rotational turbulence,
and gyrokinetic plasma turbulence.

\[[DOI](http://dx.doi.org/10.13140/RG.2.2.27072.55044)\]
\[[PDF](20230911_saxton_poster2x.pdf)\]
2023-09-11 [GAFDEM](https://gafdem.sciencesconf.org/), Nice, France.

---
