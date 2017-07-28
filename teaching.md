---
layout: page
title: Teaching
rank: 2
---
{:.no_toc}

* ToC
{:toc}

---

## Current Teaching: Qualifying Exam Review
{% assign posts = site.teaching | where:"category","qual-info"%}
<div>
{% for post in posts %} 
	{{ post.excerpt }}	
	<a href = "{{ site.baseurl }}{{ post.url}}">More...</a>
{% endfor %}
</div>

---

## Recent Posts
{% assign posts = site.teaching | where:"category","qual"%}
<div>
{% for post in posts reversed limit:2%} 
	<p>
		<span style = "display:block;text-align:center;font-style:italic;">{{ post.title }}</span>
		{{ post.excerpt }}	
		<a style = "display:block;text-align:right" href = "{{ site.baseurl }}{{ post.url}}">Read More...</a>
	</p> 
{% endfor %}
</div>

---
<!--
## Tutorial Videos

--- 

## Previous Courses

Materials from past courses e.g. exams, handouts, etc. 

---

## Misc Teaching

Lecture slides on GPU programming, LaTeX.

Misc things like LA-to-FA 

---

## Teaching Philosophy

Blog post on iterative learning, something something

---
-->


