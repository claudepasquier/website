+++
# Project title.
title = "PRED-TMR2"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Identification of transmembrane proteins."

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
links = [{name="Go to Project Site", url = "http://athina.biol.uoa.gr/PRED-TMR2/"}, {name="Execute Online", url="http://athina.biol.uoa.gr/PRED-TMR2/input.html"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Dependency graph of the sentence '*mir1 inhibits gastric cancer cell proliferation and migration by targeting MET*'"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

| PRED-TMR2      |                              |
| -------------- | ---------------------------- |
| Release date   | 1999                         |
| Implementation | C++                          |
| Authors        | Pasquier, C., Hamodrakas, S. |

PRED-TMR2[^Pasquier1999b] [^Pasquier1999c] is a new version of PRED-TMR with protein classification
capabilities. This software uses a simple artificial neural network
which classifies proteins into two classes from their sequences alone:
the membrane protein class and the non-membrane protein class. This may
be important in the functional assignment and analysis of open reading
frames (ORF's) identified in complete genomes and, especially, those
ORF's that correspond to proteins with unknown function. The network
used here has a simple hierarchical feed-forward topology and a limited
number of neurons which makes it very fast. By using only information
contained in 11 protein sequences, the method was able to identify, with
100% accuracy, all membrane proteins with reliable topologies collected
from several papers in the literature. Applied to a test set of 995
globular, water-soluble proteins, the neural network classified falsely
23 of them in the membrane protein class (97.7% of correct assignment).
The method was also applied to the complete SWISS-PROT database with
considerable success and on ORF's of several complete genomes.

#### Related publications
[^Pasquier1999b]: {{< cite page="/publication/Pasquier1999b" view="4" >}}
[^Pasquier1999c]: {{< cite page="/publication/Pasquier1999c" view="4" >}}


