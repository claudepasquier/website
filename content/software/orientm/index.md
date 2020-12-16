+++
# Project title.
title = "OrienTM"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Topology prediction of transmembrane proteins."

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
links = [{name="Go to Project Site", url = "http://athina.biol.uoa.gr/OrienTM/"}, {name="Execute Online", url="http://athina.biol.uoa.gr/OrienTM/submit.html"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Dependency graph of the sentence '*mir1 inhibits gastric cancer cell proliferation and migration by targeting MET*'"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

| OrienTM        |                                                   |
| -------------- | ------------------------------------------------- |
| Release date   | 1999                                              |
| Implementation | C++                                               |
| Authors        | Liakopoulos, T., Pasquier, C., and Hamodrakas, S. |

OrienTM[^Liakopoulos1999] [^Liakopoulos2001a] is a computer software that utilizes an initial definition of
transmembrane segments to predict the topology of transmembrane proteins
from their sequence. It uses position-specific statistical information
for amino acid residues which belong to putative non-transmembrane
segments derived from statistical analysis of non-transmembrane regions
of membrane proteins stored in the SwissProt database. Its accuracy
compares well with that of other popular existing methods.

#### Related publications
[^Liakopoulos1999]: {{< cite page="/publication/Liakopoulos1999" view="4" >}}
[^Liakopoulos2001a]: {{< cite page="/publication/Liakopoulos2001a" view="4" >}}


