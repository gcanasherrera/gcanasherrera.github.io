---
layout: page
permalink: /software/
title: software
description: Open-source software for precision cosmology.
nav: true
nav_order: 3
---

<div class="software-page">

<p class="software-intro">
My goal is to deliver the next generation of precision cosmology results with the incoming Stage IV surveys. Over the last decade I have been involved in the development, verification and validation of the ESA Euclid mission, and along the way I have built new software to go from a cosmological model to predictions for the observables, from predictions to likelihoods, and from Euclid data products to parameter constraints we can trust.
</p>

<p class="software-intro">
I have always kept in mind that the best cosmological constraints we will ever achieve will come from combining several surveys and data sets, not from any single one. That is why I make sure the software I develop is transferable and can be extended and applied to other experiments. Everything I do is open source, and most of it is built together with colleagues in the community (I am proudly a team player). If you use it, break it or want to improve it, I'd love to hear from you.
</p>

<p class="software-cta">
  <a class="btn btn-sm software-btn" href="https://github.com/gcanasherrera" target="_blank"><i class="fa-brands fa-github"></i> gcanasherrera</a>
  <a class="btn btn-sm software-btn" href="https://github.com/cloe-org" target="_blank"><i class="fa-brands fa-github"></i> cloe-org</a>
  <a class="btn btn-sm software-btn" href="https://github.com/euclidlib" target="_blank"><i class="fa-brands fa-github"></i> euclidlib</a>
</p>

<h2>cloe-org: the Euclid likelihood ecosystem</h2>

<p>
CLOE (Cosmology Likelihood for Observables in Euclid) is how Euclid goes from data to cosmological parameters. At the end of 2023 it was scientifically trusted but difficult to work with: years of technical debt meant every change felt risky, and turning scientific ideas into working projects had become exhausting. To do excellent science with Euclid's data, we needed to rethink how we built our tools. In a field already full of inference codes, we needed to do things better. That is how <a href="https://github.com/cloe-org" target="_blank">cloe-org</a> was born.
</p>

<p>
Today cloe-org is building a fully differentiable inference framework for large-scale structure cosmology and beyond: open source, modular, written in modern Python and adopted by the Euclid Consortium. It has more than 80 contributors, around 2,000 downloads every week, and papers on arXiv. Beyond cloelib and cloelike, the ecosystem includes tools for running chains at scale, blinding, figures of merit and easy installation.
</p>

<p>
cloe-org is my little joy. It grew out of countless late nights, long discussions and difficult conversations, and above all out of the support of Euclid's younger community, who never let me down, and of the senior mentors who pushed this vision with us. What started as a difficult technical problem has become a community I am genuinely proud of, and this is just the beginning.
</p>

<div class="software-card">
  <div class="software-logo software-logo-icon"><i class="fa-solid fa-atom"></i></div>
  <div class="software-body">
    <h5><a href="https://github.com/cloe-org/cloelib" target="_blank">cloelib</a> <span class="software-role">creator &amp; lead developer</span></h5>
    <p>The theory library. It computes Euclid observables (angular power spectra, correlation functions, COSEBIs and spectroscopic multipoles) from any cosmology, using Boltzmann solvers and emulators such as CAMB, CLASS, EuclidEmulator2, BACCO, CosmoPower-JAX or COMET through a common interface.</p>
    <pre class="software-install"><code>pip install cloelib</code></pre>
    <p class="software-links">
      <a href="https://github.com/cloe-org/cloelib" target="_blank"><i class="fa-brands fa-github"></i> code</a>
      <a href="https://pypi.org/project/cloelib/" target="_blank"><i class="fa-brands fa-python"></i> PyPI</a>
      <a href="https://arxiv.org/abs/2605.23839" target="_blank"><i class="fa-solid fa-file-lines"></i> paper</a>
    </p>
  </div>
</div>

<div class="software-card">
  <div class="software-logo"><img src="{{ '/assets/img/software/cloelike.png' | relative_url }}" alt="cloelike logo" loading="lazy"></div>
  <div class="software-body">
    <h5><a href="https://github.com/cloe-org/cloelike" target="_blank">cloelike</a> <span class="software-role">creator &amp; lead developer</span></h5>
    <p>The likelihoods, built on cloelib. It covers all Euclid primary probes: photometric 3×2pt in harmonic and real space, BNT C(ℓ), COSEBIs, and spectroscopic full-shape and BAO, separately or combined. Installing it gives you the whole stack.</p>
    <pre class="software-install"><code>pip install cloelike</code></pre>
    <p class="software-links">
      <a href="https://github.com/cloe-org/cloelike" target="_blank"><i class="fa-brands fa-github"></i> code</a>
      <a href="https://pypi.org/project/cloelike/" target="_blank"><i class="fa-brands fa-python"></i> PyPI</a>
      <a href="https://arxiv.org/abs/2605.23841" target="_blank"><i class="fa-solid fa-file-lines"></i> paper</a>
    </p>
  </div>
</div>

<div class="software-card">
  <div class="software-logo"><img src="{{ '/assets/img/software/cloe.png' | relative_url }}" alt="CLOE logo" loading="lazy"></div>
  <div class="software-body">
    <h5><a href="https://github.com/cloe-org/CLOE" target="_blank">CLOE</a> <span class="software-role">core developer</span></h5>
    <p>The original Euclid Consortium likelihood code, which we used for the official Euclid forecasts and validation. cloelib and cloelike grew out of it.</p>
    <p class="software-links">
      <a href="https://github.com/cloe-org/CLOE" target="_blank"><i class="fa-brands fa-github"></i> code</a>
    </p>
  </div>
</div>

<h2>Euclid data and statistics</h2>

<div class="software-card">
  <div class="software-logo"><img src="{{ '/assets/img/software/euclidlib.png' | relative_url }}" alt="euclidlib logo" loading="lazy"></div>
  <div class="software-body">
    <h5><a href="https://github.com/euclidlib/euclidlib" target="_blank">euclidlib</a> <span class="software-role">core developer</span></h5>
    <p>A community Python library for reading Euclid's cosmology-ready data products, such as redshift distributions, two-point statistics and covariances, so you can spend your time on the science instead of the file formats.</p>
    <pre class="software-install"><code>pip install euclidlib</code></pre>
    <p class="software-links">
      <a href="https://github.com/euclidlib/euclidlib" target="_blank"><i class="fa-brands fa-github"></i> code</a>
      <a href="https://pypi.org/project/euclidlib/" target="_blank"><i class="fa-brands fa-python"></i> PyPI</a>
    </p>
  </div>
</div>

<div class="software-card">
  <div class="software-logo"><img src="{{ '/assets/img/software/darkflipper.png' | relative_url }}" alt="darkflipper logo" loading="lazy"></div>
  <div class="software-body">
    <h5><a href="https://github.com/cloe-org/darkflipper" target="_blank">darkflipper</a> <span class="software-role">creator</span></h5>
    <p>Figures of Merit, Figures of Bias, p-values and other diagnostics I kept re-implementing for systematics studies, now in one place with clear definitions.</p>
    <pre class="software-install"><code>pip install darkflipper</code></pre>
    <p class="software-links">
      <a href="https://github.com/cloe-org/darkflipper" target="_blank"><i class="fa-brands fa-github"></i> code</a>
      <a href="https://pypi.org/project/darkflipper/" target="_blank"><i class="fa-brands fa-python"></i> PyPI</a>
    </p>
  </div>
</div>

<h2>Teaching and reproducibility</h2>

<div class="software-card">
  <div class="software-logo software-logo-icon"><i class="fa-solid fa-chalkboard-user"></i></div>
  <div class="software-body">
    <h5><a href="https://github.com/gcanasherrera/Stats4Cosmology" target="_blank">Stats4Cosmology</a></h5>
    <p>The notebooks I use to teach statistics for cosmology: from measuring H₀ with supernovae to running cosmological chains and comparing models with Cobaya.</p>
    <p class="software-links">
      <a href="https://github.com/gcanasherrera/Stats4Cosmology" target="_blank"><i class="fa-brands fa-github"></i> code</a>
      <a href="https://doi.org/10.5281/zenodo.13614370" target="_blank"><i class="fa-solid fa-fingerprint"></i> DOI</a>
    </p>
  </div>
</div>

<div class="software-card">
  <div class="software-logo software-logo-icon"><i class="fa-solid fa-chart-line"></i></div>
  <div class="software-body">
    <h5><a href="https://github.com/gcanasherrera/Forecasting-Euclid" target="_blank">Forecasting-Euclid</a></h5>
    <p>All the scripts and notebooks behind our forecasts for Euclid's end-of-mission (DR3) cosmological constraints, so anyone can rerun them.</p>
    <p class="software-links">
      <a href="https://github.com/gcanasherrera/Forecasting-Euclid" target="_blank"><i class="fa-brands fa-github"></i> code</a>
      <a href="https://arxiv.org/abs/2510.09153" target="_blank"><i class="fa-solid fa-file-lines"></i> paper</a>
    </p>
  </div>
</div>

</div>

<style>
.software-page h2 {
  margin-top: 2.5rem;
  margin-bottom: 1rem;
  color: var(--global-theme-color);
  border-bottom: 2px solid var(--global-divider-color);
  padding-bottom: 0.5rem;
}

.software-page .software-intro {
  font-size: 1.05rem;
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
}

.software-page .software-btn i {
  margin-right: 0.35rem;
}

.software-page .software-card {
  display: flex;
  gap: 1.25rem;
  align-items: flex-start;
  padding: 1.25rem;
  margin-bottom: 1.25rem;
  border: 1px solid var(--global-divider-color);
  border-radius: 0.5rem;
  background: var(--global-card-bg-color);
  box-shadow: 0 2px 4px rgba(0,0,0,0.05);
  transition: transform 0.2s, box-shadow 0.2s;
}

.software-page .software-card:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

.software-page .software-logo {
  flex: 0 0 88px;
  width: 88px;
  height: 88px;
  border-radius: 0.75rem;
  background: #fff;
  border: 1px solid var(--global-divider-color);
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}

.software-page .software-logo img {
  width: 100%;
  height: 100%;
  object-fit: contain;
}

.software-page .software-logo-icon {
  background: transparent;
  border: 2px solid var(--global-theme-color);
  color: var(--global-theme-color);
  font-size: 2.2rem;
}

.software-page .software-body {
  flex: 1;
  min-width: 0;
}

.software-page .software-body h5 {
  margin-bottom: 0.5rem;
}

.software-page .software-role {
  display: inline-block;
  font-size: 0.7rem;
  font-weight: 500;
  vertical-align: middle;
  margin-left: 0.4rem;
  padding: 0.15rem 0.5rem;
  border-radius: 999px;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  border: 1px solid var(--global-theme-color);
  color: var(--global-theme-color);
}

.software-page .software-install {
  margin: 0.5rem 0 0.75rem;
  padding: 0.4rem 0.75rem;
  font-size: 0.85rem;
}

.software-page .software-links {
  margin-bottom: 0;
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

@media (max-width: 576px) {
  .software-page .software-card {
    flex-direction: column;
  }

  .software-page .software-logo {
    width: 64px;
    height: 64px;
    flex-basis: 64px;
  }
}
</style>
