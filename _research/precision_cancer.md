---
layout: post
title: Quantifying Uncertainties in Predictive Medicine
category: rfchemo
---

One of the major scientific goals of the 21st century is to make medicine _personalized_ and _predictive_.  A major role will be played by mathematical models of diseases and treatments, which can provide personalized predictions when coupled with patient-specific measurements such as imaging data and genomics.  The goal of this project is to use mathematical and numerical simulation techniques to understand uncertainties that arise when emission imaging data is used in predictive models of treatment efficacy.

<!--more-->
---

{:.no_toc}

* ToC
{:toc}
### Predictive Tasks

What patient-specific information is actually gained through noisy emission imaging, and how can this information be used in predictive models?  How reliable are predictions made with this data? How practical is personalized, predictive medicine?  

Before we answer any of these questions

--- 

### Random Field Modeling
\\(
\newcommand{\r}{\boldsymbol{r}}
\newcommand{\s}{\hat{\boldsymbol{s}}}
\newcommand{\K}{\mathcal{K}}
\\)

One of the main mathematical objects in this project is the _random field_.  A random field is a random spatiotemporal function or generalized function $f(\boldsymbol{r},t;\omega)$.  Random means that for any collection of test functions $\Phi = (\varphi_1,\ldots,\varphi_n)$, 

$$
X_\Phi = \left[\langle f,\varphi_1\rangle,\ldots,\langle f,\varphi_n\rangle\right]^T
$$ 

is an $n$-dimensional random vector.  Why do we need random fields?  Because each patient is different, anatomy is spatially and temporally heterogenous, and imaging systems are noisy! 

![]({{site.baseurl}}/assets/research/all_mias_kl_draws.png){: .center-image width="500px"}


--- 

### The Role of Emission Tomography


