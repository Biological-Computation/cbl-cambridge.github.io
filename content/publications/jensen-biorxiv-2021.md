---
date: 2021-06-17T10:03:31+01:00
title: "Scalable Bayesian GPFA with automatic relevance determination and discrete noise models"
authors: ["ktj21<sup>*</sup>", "tck29<sup>*</sup>", "jts58", "gjeh2"]
year: "2021"
publication: "NeurIPS"
type: "rconf" # journal / rconf (i.e. refereed conference) / uconf (i.e. unrefereed conference) / thesis / preprint / workshop
link: "https://proceedings.neurips.cc/paper/2021/hash/58238e9ae2dd305d79c2ebc8c1883422-Abstract.html"
file: "" # IF you are NOT able to provide a link, then place a pdf in static/publications/ and write the filename here (e.g. "hennequin-neuron-2018.pdf") 
code: "" # link to e.g. github repo
illustration: "" # place image (e.g. cover) in static/publications/
selected: false # (ignore for now; in the future we might want to add a "Selected publications" section)
labs: ["hennequin"] # list of labs on which the publication should be displayed (use "cbl" to display on the main CBL website, and the PI's lastname (lowercase) for individual lab's websites, e.g. "hennequin")
draft: false
---

Latent variable models are ubiquitous in the exploratory analysis of neural
population recordings, where they allow researchers to summarize the activity
of large populations of neurons in lower dimensional ‘latent’ spaces.
Existing methods can generally be categorized into (i) Bayesian methods that
facilitate flexible incorporation of prior knowledge and uncertainty
estimation, but which typically do not scale to large datasets; and (ii)
highly parameterized methods without explicit priors that scale better but
often struggle in the low-data regime. Here, we bridge this gap by developing
a fully Bayesian yet scalable version of Gaussian process factor analysis
(bGPFA) which models neural data as arising from a set of inferred latent
processes with a prior that encourages smoothness over time. Additionally,
bGPFA uses automatic relevance determination to infer the dimensionality of
neural activity directly from the training data during optimization. To
enable the analysis of continuous recordings without trial structure, we
introduce a novel variational inference strategy that scales near-linearly in
time and also allows for non-Gaussian noise models more appropriate for
electrophysiological recordings. We apply bGPFA to continuous recordings
spanning 30 minutes with over 14 million data points from primate motor and
somatosensory cortices during a self-paced reaching task. We show that neural
activity progresses from an initial state at target onset to a reach-specific
preparatory state well before movement onset. The distance between these
initial and preparatory latent states is predictive of reaction times across
reaches, suggesting that such preparatory dynamics have behavioral relevance
despite the lack of externally imposed delay periods. Additionally, bGPFA
discovers latent processes that evolve over slow timescales on the order of
several seconds and contain complementary information about reaction time.
These timescales are longer than those revealed by methods which focus on
individual movement epochs and may reflect fluctuations in e.g. task
engagement.
