---
layout: page
title: Research
rank: 1
---

I am a mathematician and computational scientist working to understand how noisy imaging data can be used to rigorously make decisions in medicine.  My research involves several mathematical topics, including image science and statistical inverse problems, uncertainty quantification, theoretical and computational statistical decision theory, mathematical modeling of physical and biological systems, and Monte Carlo methods.  The project that I'm currently most excited about concerns the mathematical, statistical and computational issues that arise when noisy molecular imaging data is used to help predict treatment outcomes in personalized cancer therapy.  Abstractly, the major theme that drives my research program is making predictions in complex, dynamic, multi-scale systems when only imprecise and indirect data about the system is known.

To read more about specific projects, see below!

---

## Projects
{:.no_toc}

* ToC
{:toc}

---

### Quantifying uncertainties in predictive medicine
{% assign posts = site.research | where:"category","rfchemo"%}
<div>
{% for post in posts %} 
	{{ post.excerpt }}	
	<a href = "{{ site.baseurl }}{{ post.url}}">Read more</a>
{% endfor %}
</div>

---

### Image science with particle processing detectors
{% assign posts = site.research | where:"category","pp"%}

<div>
{% for post in posts %} 
	{{ post.excerpt }}	
	<a href = "{{ site.baseurl }}{{ post.url}}">Read more</a>
{% endfor %}
</div>

---

### High performance parallel numerical simulation of imaging systems

---

### Task-based assessment of image quality

---

### Sparsity based methods in image science 











