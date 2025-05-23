+++
# Project title.
title = "AllOnto"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Triple store with OWL query answering."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Semantic Data Integration", "Computational Biology"]

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

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Dependency graph of the sentence '*mir1 inhibits gastric cancer cell proliferation and migration by targeting MET*'"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

| AllOnto        |             |
| -------------- | ----------- |
| Release date   | 2008        |
| Implementation | Java        |
| Author         | Pasquier C. |



AllOnto[^Pasquier2008a] [^Pasquier2011] is a Knowledge Base System capable of storing and performing
queries on a large set of RDF/OWL specifications (including the storing
and querying of reified statements). It includes reasoning capabilities
like type inference, transitivity and the handling of these two OWL
constructs: "sameAs" and "inverseOf". In addition, it is capable of
storing and querying the provenance of information.

#### Related publications
[^Pasquier2008a]: {{< cite page="/publication/Pasquier2008a" view="4" >}}
[^Pasquier2011]: {{< cite page="/publication/Pasquier2011" view="4" >}}

