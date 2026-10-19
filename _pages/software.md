---
layout: page
permalink: /software/
title: software
description: Open-source tools for precision cosmology, from Euclid pixels to posteriors.
nav: true
nav_order: 3
---

<div class="software-page">

<p class="lead software-intro">
Euclid will map a third of the sky and billions of galaxies. Turning that map into answers about <strong>dark matter</strong>, <strong>dark energy</strong> and <strong>gravity</strong> takes more than data: it takes fast, tested and open software. I build that software in the open, with the community, so that every number in a Euclid cosmology paper can be checked, reproduced and improved by anyone.
</p>

<p class="software-cta">
  <a class="btn btn-sm software-btn" href="https://github.com/gcanasherrera" target="_blank"><i class="fa-brands fa-github"></i> github.com/gcanasherrera</a>
  <a class="btn btn-sm software-btn" href="https://github.com/cloe-org" target="_blank"><i class="fa-solid fa-sitemap"></i> cloe-org</a>
  <a class="btn btn-sm software-btn" href="https://github.com/euclidlib" target="_blank"><i class="fa-solid fa-satellite"></i> euclidlib</a>
</p>

## <i class="fa-solid fa-infinity"></i> The CLOE ecosystem

<p>The next generation of the <em>Cosmology Likelihood for Observables in Euclid</em>: a modular, pip-installable stack that takes you from cosmological parameters to Euclid likelihoods for every primary probe.</p>

<div class="row mt-3">

<div class="col-md-12 mb-4">
  <div class="card h-100 software-card software-card-featured">
    <div class="card-body">
      <h5 class="card-title"><i class="fa-solid fa-atom"></i> <a href="https://github.com/cloe-org/cloelib" target="_blank">cloelib</a> <span class="badge software-role">creator &amp; lead developer</span></h5>
      <p class="card-text software-tagline">The theory engine behind Euclid cosmology.</p>
      <p class="card-text">Euclid-like observables (angular power spectra, correlation functions, COSEBIs, spectroscopic multipoles) in minutes. It plugs into Boltzmann solvers and emulators (CAMB, CLASS, EuclidEmulator2, BACCO, CosmoPower-JAX, COMET and more) through clean Python protocols, and ships with a JAX playground for gradient-based inference.</p>
      <pre class="software-install"><code>pip install cloelib</code></pre>
      <p class="card-text software-links">
        <a href="https://github.com/cloe-org/cloelib" target="_blank"><i class="fa-brands fa-github"></i> code</a>
        <a href="https://pypi.org/project/cloelib/" target="_blank"><i class="fa-brands fa-python"></i> PyPI</a>
        <a href="https://arxiv.org/abs/2605.23839" target="_blank"><i class="fa-solid fa-file-lines"></i> paper</a>
      </p>
    </div>
  </div>
</div>

<div class="col-md-6 mb-4">
  <div class="card h-100 software-card">
    <div class="card-body">
      <h5 class="card-title"><i class="fa-solid fa-scale-balanced"></i> <a href="https://github.com/cloe-org/cloelike" target="_blank">cloelike</a> <span class="badge software-role">creator &amp; lead developer</span></h5>
      <p class="card-text software-tagline">Where theory meets Euclid data.</p>
      <p class="card-text">Likelihoods for all Euclid primary probes: 3×2pt in harmonic and real space, BNT C(ℓ), COSEBIs, spectroscopic full-shape and BAO, and their joint analysis. One <code>pip install</code> brings in the whole stack.</p>
      <pre class="software-install"><code>pip install cloelike</code></pre>
      <p class="card-text software-links">
        <a href="https://github.com/cloe-org/cloelike" target="_blank"><i class="fa-brands fa-github"></i> code</a>
        <a href="https://pypi.org/project/cloelike/" target="_blank"><i class="fa-brands fa-python"></i> PyPI</a>
        <a href="https://arxiv.org/abs/2605.23841" target="_blank"><i class="fa-solid fa-file-lines"></i> paper</a>
      </p>
    </div>
  </div>
</div>

<div class="col-md-6 mb-4">
  <div class="card h-100 software-card">
    <div class="card-body">
      <h5 class="card-title"><i class="fa-solid fa-landmark"></i> <a href="https://github.com/cloe-org/CLOE" target="_blank">CLOE</a> <span class="badge software-role">core developer</span></h5>
      <p class="card-text software-tagline">The original Euclid likelihood.</p>
      <p class="card-text">The Euclid Consortium code that set the standard for combined photometric and spectroscopic analyses and powered the official Euclid forecasts and validation campaigns. It is the foundation the new ecosystem is built on.</p>
      <p class="card-text software-links">
        <a href="https://github.com/cloe-org/CLOE" target="_blank"><i class="fa-brands fa-github"></i> code</a>
      </p>
    </div>
  </div>
</div>

</div>

## <i class="fa-solid fa-satellite-dish"></i> Euclid data &amp; statistics

<div class="row mt-3">

<div class="col-md-6 mb-4">
  <div class="card h-100 software-card">
    <div class="card-body">
      <h5 class="card-title"><i class="fa-solid fa-database"></i> <a href="https://github.com/euclidlib/euclidlib" target="_blank">euclidlib</a> <span class="badge software-role">core developer</span></h5>
      <p class="card-text software-tagline">Euclid data, ready for science in one line.</p>
      <p class="card-text">A community Python library for reading Euclid's cosmology-ready data products (redshift distributions, two-point statistics, covariances and more) without wrestling with file formats.</p>
      <pre class="software-install"><code>pip install euclidlib</code></pre>
      <p class="card-text software-links">
        <a href="https://github.com/euclidlib/euclidlib" target="_blank"><i class="fa-brands fa-github"></i> code</a>
        <a href="https://pypi.org/project/euclidlib/" target="_blank"><i class="fa-brands fa-python"></i> PyPI</a>
      </p>
    </div>
  </div>
</div>

<div class="col-md-6 mb-4">
  <div class="card h-100 software-card">
    <div class="card-body">
      <h5 class="card-title"><i class="fa-solid fa-fish"></i> <a href="https://github.com/cloe-org/darkflipper" target="_blank">darkflipper</a> <span class="badge software-role">creator</span></h5>
      <p class="card-text software-tagline">Flip the dark side of statistics in cosmology.</p>
      <p class="card-text">Figures of Merit, Figures of Bias, p-values and tension metrics, with consistent definitions, so systematics studies are robust, transparent and publication-ready.</p>
      <pre class="software-install"><code>pip install darkflipper</code></pre>
      <p class="card-text software-links">
        <a href="https://github.com/cloe-org/darkflipper" target="_blank"><i class="fa-brands fa-github"></i> code</a>
        <a href="https://pypi.org/project/darkflipper/" target="_blank"><i class="fa-brands fa-python"></i> PyPI</a>
      </p>
    </div>
  </div>
</div>

</div>

## <i class="fa-solid fa-book-open"></i> Open science &amp; teaching

<div class="row mt-3">

<div class="col-md-6 mb-4">
  <div class="card h-100 software-card">
    <div class="card-body">
      <h5 class="card-title"><i class="fa-solid fa-chalkboard-user"></i> <a href="https://github.com/gcanasherrera/Stats4Cosmology" target="_blank">Stats4Cosmology</a></h5>
      <p class="card-text software-tagline">Learn Bayesian cosmology by doing it.</p>
      <p class="card-text">Hands-on notebooks covering everything from measuring H₀ with supernovae to running full cosmology chains and model comparison with Cobaya.</p>
      <p class="card-text software-links">
        <a href="https://github.com/gcanasherrera/Stats4Cosmology" target="_blank"><i class="fa-brands fa-github"></i> code</a>
        <a href="https://doi.org/10.5281/zenodo.13614370" target="_blank"><i class="fa-solid fa-fingerprint"></i> DOI</a>
      </p>
    </div>
  </div>
</div>

<div class="col-md-6 mb-4">
  <div class="card h-100 software-card">
    <div class="card-body">
      <h5 class="card-title"><i class="fa-solid fa-chart-line"></i> <a href="https://github.com/gcanasherrera/Forecasting-Euclid" target="_blank">Forecasting-Euclid</a></h5>
      <p class="card-text software-tagline">Euclid's final constraints, fully reproducible.</p>
      <p class="card-text">The scripts and notebooks behind the Euclid DR3 end-of-mission forecasts, from CLOE likelihoods to Nautilus posteriors.</p>
      <p class="card-text software-links">
        <a href="https://github.com/gcanasherrera/Forecasting-Euclid" target="_blank"><i class="fa-brands fa-github"></i> code</a>
        <a href="https://arxiv.org/abs/2510.09153" target="_blank"><i class="fa-solid fa-file-lines"></i> paper</a>
      </p>
    </div>
  </div>
</div>

</div>

<p class="software-outro">
<i class="fa-solid fa-hand-holding-heart"></i> All of these projects are open source and welcome contributions. Found a bug, want a new feature or just want to say hi? Open an issue or start a discussion on <a href="https://github.com/gcanasherrera" target="_blank">GitHub</a>.
</p>

</div>

<style>
.software-page h2 {
  margin-top: 2.5rem;
  margin-bottom: 1rem;
  color: var(--global-theme-color);
  border-bottom: 2px solid var(--global-divider-color);
  padding-bottom: 0.5rem;
}

.software-page h2 i,
.software-page .card-title i,
.software-page .software-outro i {
  color: var(--global-theme-color);
  margin-right: 0.5rem;
}

.software-page .software-intro {
  font-size: 1.1rem;
  line-height: 1.7;
}

.software-page .software-cta {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin: 1.25rem 0 0.5rem;
}

.software-page .software-btn {
  border: 1px solid var(--global-theme-color);
  color: var(--global-theme-color);
  border-radius: 999px;
  padding: 0.3rem 0.9rem;
}

.software-page .software-btn:hover {
  background: var(--global-theme-color);
  color: var(--global-hover-text-color, #fff);
  border-bottom-color: var(--global-theme-color);
}

.software-page .software-btn i {
  margin-right: 0.35rem;
}

.software-page .card {
  border: 1px solid var(--global-divider-color);
  box-shadow: 0 2px 4px rgba(0,0,0,0.05);
  transition: transform 0.2s, box-shadow 0.2s;
}

.software-page .card:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

.software-page .software-card-featured {
  border-left: 4px solid var(--global-theme-color);
}

.software-page .software-role {
  font-size: 0.7rem;
  font-weight: 500;
  vertical-align: middle;
  margin-left: 0.4rem;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  border: 1px solid var(--global-theme-color);
  color: var(--global-theme-color);
  background: transparent;
}

.software-page .software-tagline {
  font-style: italic;
  color: var(--global-text-color-light);
}

.software-page .software-install {
  margin: 0.5rem 0 0.75rem;
  padding: 0.4rem 0.75rem;
  font-size: 0.85rem;
}

.software-page .software-links a {
  margin-right: 1rem;
  white-space: nowrap;
}

.software-page .software-links i {
  margin-right: 0.25rem;
}

.software-page a {
  color: var(--global-theme-color);
  text-decoration: none;
  border-bottom: 1px solid transparent;
  transition: border-bottom-color 0.2s;
}

.software-page a:hover {
  border-bottom-color: var(--global-theme-color);
}

.software-page .software-outro {
  margin-top: 1.5rem;
  text-align: center;
}
</style>
