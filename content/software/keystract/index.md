+++
# Project title.
title = "KeyStract"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Keywords extraction from scientific papers."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Natural Language Processing", "Ended Project"]

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
#links = [{name="Go to Project Site", url = "http://www-sop.inria.fr/lemme/Claude.Pasquier/ketuk/"}, {name="Get Code", url="data/ketuk.zip"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Dependency graph of the sentence '*mir1 inhibits gastric cancer cell proliferation and migration by targeting MET*'"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

| KeyStract      |              |
| -------------- | ------------ |
| Release date   | 2010         |
| Implementation | Java         |
| Author         | Pasquier, C. |

KeyStract is a method designed for keyphrase extraction from a single document [^Pasquier2010].
The principle of the algorithm is to cluster sentences of the documents in order to highlight parts of text that are semantically related.
The clusters of sentences, that reflect the themes of the document, are then analyzed to find the main topics of the text.
Finally, the most important words, or groups of words, from these topics are proposed as keyphrases.
This method has been evaluated on task number 5 (Automatic Keyphrase Extraction from Scientific Articles) of SemEval-2010: the 5th International Workshop on Semantic Evaluations.

#### Related publication
[^Pasquier2010]: {{< cite page="/publication/Pasquier2010" view="4" >}}

