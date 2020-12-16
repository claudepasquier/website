+++
# Project title.
title = "MiRAI"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Prediction of microRNA-disease associations."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Computational Biology", "Graph Mining", "Ended Project"]

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
links = [{name="Get Code", url="https://github.com/claudepasquier/mirai"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Dependency graph of the sentence '*mir1 inhibits gastric cancer cell proliferation and migration by targeting MET*'"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

| MiRAI          |                                  |
| -------------- | -------------------------------- |
| Release date   | version 1: 2016, version 2: 2017 |
| Implementation | Python                           |
| Authors        | Pasquier, C. and Pallez D.       |

MiRAI is a Python implementation of a method to predict associations between miRNAs and diseases [^Pasquier2016a]. MiRNAs and their associations with different pieces of knowledge were represented as a multidimentional network. It was therefore possible to represent, in this way, the known associations between miRNAs and diseases, the genes targeted by miRNAs, the physical proximity between miRNAs on the genome, the families to which miRNAs belong, etc.
MiRAI uses the concept of distributional semantics to analyze these data. The principle is to transform the multidimensional network so defined into a vector space and to use metrics on the feature space to predict associations between miRNAs and diseases.

The performance of the method was characteristic of an excellent classifier.
However, MiRAI's performance depends on many parameters that cannot be adjusted manually. We have therefore proposed an improvement in which a parallel surrogate-assisted evolutionary algorithm is proposed in order to automatically find an optimal configuration of our predictive method [^Pallez2017].

The first version of MiRAI is registered at the [Agence pour la Protection des Programmes](https://www.app.asso.fr/en) under the identifier: **IDDN.FR.001.390014.000.S.C.2018.000.31235**. 

#### Related publication
[^Pasquier2016a]: {{< cite page="/publication/Pasquier2016a" view="4" >}}
[^Pallez2017]: {{< cite page="/publication/Pallez2017" view="4" >}}

