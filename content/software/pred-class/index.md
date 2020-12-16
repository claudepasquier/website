+++
# Project title.
title = "PRED-CLASS"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Classification of proteins with a neural network."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Computational Biology", "Protein Structure Prediction", "Ended Project"]

# Optional external URL for project (replaces project detail page).
#external_link = "http://athina.biol.uoa.gr/FT/"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references 
#   `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides = "example-slides"

# Links (optional).
url_pdf = ""
url_slides = ""
url_video = ""
url_code = ""

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
#links = [{icon_pack = "fab", icon="twitter", name="Follow", url = "https://twitter.com/georgecushen"}]
links = [{name="Go to Project Site", url = "http://athina.biol.uoa.gr/PRED-CLASS/"}, {name="Execute Online", url="http://athina.biol.uoa.gr/PRED-CLASS/input.html"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Dependency graph of the sentence '*mir1 inhibits gastric cancer cell proliferation and migration by targeting MET*'"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

| PRED-CLASS     |                                                 |
| -------------- | ----------------------------------------------- |
| Release date   | 2001                                            |
| Implementation | C++                                             |
| Authors        | Pasquier, C., Promponas, V., and Hamodrakas, S. |

PRED-CLASS[^Pasquier2001] [^Promponas2001] is a cascading system of hierarchical, artificial neural
networks for the generalized classification of proteins into four
distinct classes - transmembrane, fibrous, globular, and mixed - from
information solely encoded in their amino acid sequences. The
architecture of the individual component networks is kept very simple,
reducing the number of free parameters (network synaptic weights) for
faster training, improved generalization, and the avoidance of data
overfitting. Capturing information from as few as 50 protein sequences
spread among the four target classes (6 transmembrane, 10 fibrous, 13
globular, and 17 mixed), PRED-CLASS was able to obtain 371 correct
predictions out of a set of 387 proteins (success rate 96%)
unambiguously assigned into one of the target classes. The application
of PRED-CLASS to several test sets and complete proteomes of several
organisms demonstrates that such a method could serve as a valuable tool
in the annotation of genomic open reading frames with no functional
assignment or as a preliminary step in fold recognition and ab initio
structure prediction methods.

#### Related publications
[^Pasquier2001]: {{< cite page="/publication/Pasquier2001" view="4" >}}
[^Promponas2001]: {{< cite page="/publication/Promponas2001" view="4" >}}


