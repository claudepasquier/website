+++
# Project title.
title = "GenMiner"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Mining association rule from gene expression."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Gene Expression Analysis", "Data Mining", "Ended Project"]

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
links = [{name="Download Code", url = "data/GenMiner.zip"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Dependency graph of the sentence '*mir1 inhibits gastric cancer cell proliferation and migration by targeting MET*'"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

| GenMiner       |                                              |
| -------------- | -------------------------------------------- |
| Release date   | 2008                                         |
| Implementation | Java                                         |
| Authors        | Martinez, R., Pasquier, N., and Pasquier, C. |


GenMiner [^Martinez2007] [^Martinez2008b] [^Martinez2009] is a Java implementation of the GenMiner algorithm for mining equivalence classes and minimal non-redundant association rule from gene expression data. This implementation integrates the R implementation of the Normalized Discretization method (NorDi) to preprocess gene expression data and the Java implementation of the JClose algorithm (JClose) to extract equivalence classes and minimal non-redundant association rules from these data.

#### Related publications
[^Martinez2007]: {{< cite page="/publication/Martinez2007" view="4" >}}
[^Martinez2008b]: {{< cite page="/publication/Martinez2008b" view="4" >}}
[^Martinez2009]: {{< cite page="/publication/Martinez2009" view="4" >}}

