---
layout: post
title: Image Science with Particle Processing Detectors
category: pp
---

In recent years, emission imaging systems have begun to incorporate a new detector design based on on-the-fly event attribute estimation.  These new detectors - called particle processing detectors - lead to interesting new mathematical models for imaging systems.  The goal is to quantify the performance of such detectors using the theory of inverse problems and statistical decision theory.

![]({{site.baseurl}}/assets/research/phasespace.png){: .center-image width="350px"}

<!--more-->
---
\\(
\newcommand{\r}{\boldsymbol{r}}
\newcommand{\e}{\mathcal{E}}
\newcommand{\s}{\hat{\boldsymbol{s}}}
\newcommand{\K}{\mathcal{K}}
\\)
To be more precise, I work with imaging system models that are decomposed into two operators, a _propagation_ operator \\(\mathcal{P}\\) and a _detection_ operator \\(\mathcal{D}\\).  The propogation operator models the physics of the energy used, so in my case (I work mostly in emission imaging) it's the solution operator to a Radiative Transfer Equation (RTE): 

$$\left\{\begin{array}{ll}
c_m\s\cdot\nabla w + c_m\mu w - \K w = f & (\r,\s)\in \Gamma,\; \e\in [0,\infty) \\
w(\r,\s,\e) = g(\r,\s,\e) & (\r,\s)\in \partial_-\Gamma,\;\e\in [0,\infty)
\end{array}\right.$$

(A figure describing optical phase space) 

This equation models the propagation of high-frequency light from visible up to X-Ray, and even particles like \\(\alpha\\)s and \\(\beta\\)s, in biological tissue.  Solving this equation results in the \\(\mathcal{P}\\) operator: 

$$
(\mathcal{P} f)(\r,\s,\e) = \frac{1}{c_m}\int_0^{\tau_-}f(\r-t\s)\exp\left(-\int_0^{\tau_-}\mu(\r-t^\prime\s)dt^\prime\right)dt
$$

This 

---

### Detector Modeling 

---

### 



