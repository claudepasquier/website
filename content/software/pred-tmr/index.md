+++
# Project title.
title = "PRED-TMR"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Prediction of proteins' transmembrane regions."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Computational Biology", "Protein Structure Prediction"]

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
links = [{name="Go to Project Site", url = "http://athina.biol.uoa.gr/PRED-TMR/"}, {name="Execute Online", url="http://athina.biol.uoa.gr/PRED-TMR/input.html"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Dependency graph of the sentence '*mir1 inhibits gastric cancer cell proliferation and migration by targeting MET*'"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

| PRED-TMR       |                                                                              |
| -------------- | ---------------------------------------------------------------------------- |
| Release date   | 1999                                                                         |
| Implementation | C++                                                                          |
| Authors        | Pasquier, C., Promponas, V., Palaios, G., Hamodrakas, I., and Hamodrakas, S. |

PRED-TMR[^Pasquier1999a] is a method that predicts transmembrane domains in proteins
using solely information contained in the sequence itself. The algorithm
refines a standard hydrophobicity analysis with a detection of potential
termini ("edges", starts and ends) of transmembrane regions. This
allows one both to discard highly hydrophobic regions not delimited by
clear start and end configurations and to confirm putative transmembrane
segments not distinguishable by their hydrophobic composition. The
accuracy obtained on a test set of 101 non-homologous transmembrane
proteins with reliable topologies compares well with that of other
popular existing methods. Only a slight decrease in prediction accuracy
was observed when the algorithm was applied to all transmembrane
proteins of the SwissProt database (release 35).

#### Related publication
[^Pasquier1999a]: {{< cite page="/publication/Pasquier1999a" view="4" >}}


