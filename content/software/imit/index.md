+++
# Project title.
title = "IMIT"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Mining frequent patterns in attributed trees."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Attributed Graph Mining", "Graph Mining"]

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

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Dependency graph of the sentence '*mir1 inhibits gastric cancer cell proliferation and migration by targeting MET*'"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

| IMIT           |              |
| -------------- | ------------ |
| Release date   | 2013         |
| Implementation | C++          |
| Author         | Pasquier, C. |

Mining frequent patterns in attributed trees (that we call asubtrees), which combines tree mining and itemset mining, requires
the exploration of a huge search space. To make our approach scalable, we investigate the
mining of condensed representations. For attributed trees, the classical concept of closure
involves both itemset closure and structural closure. IMIT includes the implementation of three algorithms for mining
all patterns, closed patterns w.r.t. itemsets (content) and/or structure in attributed trees [^Pasquier2013a] [^Pasquier2013b] [^Pasquier2016b]. We
show that, for low support values, mining content-closed attributed trees is a good compromise
between non-redundancy of solutions and execution time.

#### Related publication
[^Pasquier2013a]: {{< cite page="/publication/Pasquier2013a" view="4" >}}
[^Pasquier2013b]: {{< cite page="/publication/Pasquier2013b" view="4" >}}
[^Pasquier2016b]: {{< cite page="/publication/Pasquier2016b" view="4" >}}

