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

### Recent Posts
{% assign posts = site.teaching | where:"category","qual"%}
<div>
{% for post in posts limit:2%} 
	<p>
		{{ post.title }}
		{{ post.excerpt }}	
		<a href = "{{ site.baseurl }}{{ post.url}}">Read more</a>
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


