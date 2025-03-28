+++
# Project title.
title = "Dam-Bio"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Protein sequence analysis on the Web."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Computational Biology", "Protein Structure Prediction"]

# Optional external URL for project (replaces project detail page).
#external_link = ""

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
links = [{name="Go to Project Site", url = "http://athina.biol.uoa.gr/DAM-Bio/"}, {name="Execute Online", url = "http://athina.biol.uoa.gr/cgi-bin/orienTM/dambio.pl?start=1"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Dependency graph of the sentence '*mir1 inhibits gastric cancer cell proliferation and migration by targeting MET*'"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

| Dam-Bio        |                                                |
| -------------- | ---------------------------------------------- |
| Release date   | 1998                                           |
| Implementation | Java                                           |
| Authors        | Liakopoulos, T., Palaios, G., Harkiolakis, N., Promponas, V., Pasquier, C., Hamodrakas, I., Papandreou, N., Iconomidou, V., Papandreou, N., Tzafestas, E., Tzafestas, S., Eliopoulos, E., and Hamodrakas, S. |

Computational analysis of protein sequences with statistical models,
machine learning techniques or empirical rules leads to prediction of
structural and functional features of the corresponding molecules.
Taking into account the recent explosion of biological information in
terms of complete genome sequences the use of computational tools of
analysis is considered essential. Individual tools are available through
the Internet, and their performance depends on their liability and
simplicity of use. Dam-Bio [^Liakopoulos2000] [^Liakopoulos2001b] is a workspace that establishes data
trafficking towards a collection of tools, communication between them
and simple representation of the results of sequence and structure
analysis. At the sequence level, the following are offered: analysis of
periodical features, structural classification with neural networks,
prediction of secondary structure, prediction and topology of
transmembrane regions and multiple sequence alignment. At the structure
level, the creation and representation of protein structures and
three-dimensional fit is possible. The end-user is offered with a
user-friendly interface and a simple representation of the results. The
system's open and decentralized design permits the addition of new
individual modules that may reside anywhere on the Internet. Our future
plans include the development of modules for fold recognition, receptor
prediction and sequence complexity analysis. Interconnection between the
system, the individual tools and the user is established through the
HTTP protocol, the only requirement for its usage being Internet access.

#### Related publications
[^Liakopoulos2000]: {{< cite page="/publication/Liakopoulos2000" view="4" >}}
[^Liakopoulos2001b]: {{< cite page="/publication/Liakopoulos2001b" view="4" >}}

