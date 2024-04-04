<!-- .slide: data-background="assets/backdrop.webp" class="dark no-logo" -->

# A meet and greet with MICOM

### Christian Diener

<img src="assets/meduni/logo_slogan_dark.png" width="30%">

Slides: https://dienerlab.github.io/2024_micom_intro

<br><br>
<div class="footer">
<a href="https://creativecommons.org/licenses/by-sa/4.0/"><i class="bx bx-cctv"></i>CC BY-SA 4.0</a>
<a href="https://dienerlab.com"><i class="bx bxs-home"></i>dienerlab.com</a>
<a href="https://github.com/dienerlab"><i class="bx bxl-github"></i>dienerlab</a>
<a href="https://twitter.com/thaasophobia"><i class="bx bxl-twitter"></i>@thaasophobia</a>
<a href="https://mstdn.science/@thaasophobia"><i class="bx bxl-mastodon"></i>@thaasophobia</a>
</div>

---

<!-- .slide: data-background="var(--primary)" class="dark" -->

## Do we know enough of the rules to play the game?

<br><br>

Explaining the behavior of microbial communities through mechanisms by using *flux balance analysis (FBA)*.

---

## Quantifying Metabolism - Fluxes

<img src="assets/fluxes.png" width="45%">
<video width="45%" autoplay loop>
  <source src="assets/fluxes.mp4" type="video/mp4">
</video>

<div class="footnote">

video courtesy of [S. Nayyak](https://twitter.com/Na_y_ak) and [J. Iwasa](https://twitter.com/janetiwasa)

</div>

---

<!-- .slide: data-background="var(--primary)" class="dark" -->

### Why fluxes?

The following are all questions about *fluxes*, not *concentrations*:

- How much butyrate is produced by a particular microbiota?
- How much fiber is broken down by <i>Bacteroides</i> in this sample?
- How fast does this pathogen grow? (note that growth rates are also fluxes)

---

## Genome-scale metabolic models (GSMMs)

<img src="assets/reconstruction.png" width="80%">

----

### Reconstruction Approaches

<img src="assets/reconstruction_strategies.png" width="80%">

---

## The flux cone

<img src="assets/flux_cone.png" width="100%">

---

## Genome-scale metabolic models - pretty well-behaved

<img src="assets/gsmm.webp" width="100%">

<div class="footnote">

Schuetz et al. 2012, https://doi.org/10.1126/science.1216882<br>
Harcombe et al. 2013, https://doi.org/10.1371/journal.pcbi.1003091

</div>

---

## Still not unique

<img src="assets/reduction.png" width="100%">

---

## Community-scale metabolic models - pretty rowdy

<img src="assets/csmm.webp" width="100%">

<div class="footnote">

Diener et al. 2023, https://doi.org/10.1128/msystems.01270-22

</div>

----

<img src="assets/model_gephi.png" width="70%">

Genus-level metabolic model for the gut microbiome of a single individual.

---

## It's all just cones

<img src="assets/growth_cone.webp" width="60%">

---

## How to pick solutions from the growth cone

<img src="assets/strategies.webp" width="80%">

---

<img src="assets/micom_quick.png" width="100%">

That makes full community-scale metabolic models *usable*.

But even curated metabolic models for many species do not capture the full complexity of
metabolism. So are those models also *useful*?

How do we *validate* the model predictions?

---

## Is it better than the status quo?

<img src="assets/validation.png" width="100%">

186 metagenome samples from Swedish and Danish individuals.<br>
Manually curated metabolic models from the AGORA database.<br>
Import fluxes based on an average European diet.

<div class="footnote">

Diener et al. 2020, https://doi.org/10.1128/mSystems.00606-19<br>
Korem, Suez, Zeevi, Weinberger et al. 2015, https://dx.doi.org/10.1126%2Fscience.aac4812<br>
Magnúsdóttir et al., https://doi.org/10.1038/nbt.3703
</div>

---

## Limitations

- steady state assumption: can not *really* model abundance changes
- hard to link with concentration data (for instance metabolomics)
- limited by GSMM quality, many enzymes/metabolites not identified (bias towards CCM)
- can only model growth-associated processes (no toxicity or secondary metabolism)

---

<!-- .slide: data-background="var(--gray)" class="dark" -->

## Resources

Documentation: https://micom-dev.github.io/micom

ISB Microbiome Courses (usually day 2):
[2020](https://isbscience.org/microbiome2020), [2021](https://isbscience.org/microbiome2021), [2022](https://isbscience.org/microbiome2022),
[2023](https://isbscience.org/microbiome2023)

Reconstructed model databases: https://doi.org/10.5281/zenodo.7739096

Environmental media: https://github.com/micom-dev/media

---

<!-- .slide: data-background="var(--primary)" class="dark" -->

## Practical and FAQ

**Checking for probiotic engraftment and impact.**<br>
We will simulate an incoming <i>B. animalis</i> for a healthy sample from the iHMP project.

Notebook: https://colab.research.google.com/github/dienerlab/2024_micom_intro/blob/main/micom.ipynb
<br>(you will need a Google Account)

---

<!-- .slide: data-background="assets/meduni/bridges.png" -->

# Thanks! :smile:

---

## Construction of environmental media

<img src="assets/medium.png" width="90%">
