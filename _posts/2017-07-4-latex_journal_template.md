---
layout: post
title: LaTeX Research Journal and Dissertation Template
---

In this post I talk about the LaTeX journal/large document template that I use.  It follows a relatively simple structure using the `subfiles` package. I use this system for any big multi-file document like my research journal, dissertation, and software documentation.  It allows separate compilation of subfiles, which makes it easy to quickly work on components in isolation.

<!--more-->
{:.no_toc}

* ToC
{:toc}

---

### Code 
You can clone the git repository or download a zip of the template <a href="https://github.com/nhenscheid/latexjournaltemplate" target="_blank">here</a>.  

Example compiled final document and subfiles:  <a href="/site/assets/latex/journal_template.pdf" target="_blank">Main file</a>, <a href="/site/assets/latex/math.pdf" target="_blank">First subfile</a>, <a href="/site/assets/latex/physics.pdf" target="_blank">Second subfile</a>

### Structure 
The project is separated into folders, usually one folder per subfile (you can have multiple subfiles in a folder if you want).  For example, in the template, I have provided three folders: a `main` folder that contains the main LaTeX file, a stylesheet, and bibliography, then two folders for two subfiles, one called `math` and one called `physics`.

<UL>
  <LI>main</LI>
  <UL>
    <LI>journal_template.tex</LI>
    <LI>journal_template_bib.bib</LI>
    <LI>journal_template_style.sty</LI>
  </UL>
  <LI>math</LI>
  <UL>
    <LI>figures</LI>
    <UL>
      <LI>riemann.png</LI>
    </UL>
    <LI>math.tex</LI>
  </UL>
  
  <LI>physics</LI>
  <UL>
    <LI>figures</LI>
    <UL><LI>LIGO.png</LI></UL>
    <LI>physics.tex</LI>
  </UL>
</UL>


Note that the folders for the subfiles are at the same level as the main folder.  Within each subfolder, you can have as many additional subfolders as you like to organize files.  The only caveat is you have to provide links relative to the base folder.  This is explained in more detail in each subfile (`math.tex` and `physics.tex`). 

--- 

### Compilation
If set up correctly, you should be able to compile any of the `.tex` files as you normally would, either separately (i.e. only `math.tex`) or the main file (`main.tex`).  This is the main advantage of the system - it allows you to work on smaller parts of a big document without needing to compile the whole file.  You can also compile bibliographies in the subfiles (using the standard routine) and they will show in the subfiles.  When you compile the main file with bibliography, it will only put a bibliography at the end, not after each subfile.  This is explained in the comments in `math.tex` and `physics.tex`
