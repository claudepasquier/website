+++
# Project title.
title = "CGGA"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Extraction of bi-clusters of genes."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Gene Expression Analysis", "Data Mining", "Ended Project"]

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
links = [{name="Download Binary", url = "data/CGGA.zip"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Dependency graph of the sentence '*mir1 inhibits gastric cancer cell proliferation and migration by targeting MET*'"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

| CGGA           | (Co-expressed Gene Groups Analysis)          |
| -------------- | -------------------------------------------- |
| Release date   | 2006                                         |
| Implementation | R                                            |
| Authors        | Martinez, R., Pasquier, N., and Pasquier, C. |
| Availability   | binary downloadable [here](data/CGGA.zip)         |

CGGA (Co-expressed Gene Groups Analysis) [^Martinez2006] [^Martinez2006a] [^Martinez2006b] [^Martinez2008a] performs the extraction of bi-clusters of co-regulated genes from integrated gene expression data and gene annotations obtained from biological knowledge.
First, the gene rank hierarchy is constructed using SAM F-Scores and then, the CGGA algorithm is applied to group of co-expressed genes.


#### Related publications
[^Martinez2006]: {{< cite page="/publication/Martinez2006" view="4" >}}
[^Martinez2006a]: {{< cite page="/publication/Martinez2006a" view="4" >}}
[^Martinez2006b]: {{< cite page="/publication/Martinez2006b" view="4" >}}
[^Martinez2008a]: {{< cite page="/publication/Martinez2008a" view="4" >}}

