+++
# Project title.
title="Prototype-based Programming"

# Date this page was created.
date = "2019-10-24T00:00:00"

# Project summary to display on homepage.
summary = "Dynamic document sharing based on delegation and cloning."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Software Engineering", "Structured Documents", "Ended Project"]

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
  caption = "View of the structured document editor being part of the BIBLE system."
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

#### Active from 1990 to 1994

## Research rationale
Little research was devoted to the theme of the representation and handling of structured documents.
However, one realizes that there is still a lot of work to be done when one considers that computer programs are a simplified form of documents for which there are already problems of organization, sharing, interpretation, generation or dynamic modification.
As with programs, the processing of structured documents requires the use of abstract grammars to define the syntactic and semantic rules of their composition.
In addition, the introduction of active structured documents (i.e. whose abstract representation can evolve dynamically) requires the implementation of mechanisms to organize the different document models and to describe the evolution of several versions of the same document.
There are also crucial questions about the reuse of documents and their interoperability in the case of heterogeneous systems [@Pasquier1991].

## Results

#### A system to provide dynamic document sharing based on delegation and cloning

My PhD thesis work aimed to explore the use of software engineering fundamentals to define the basis for the representation and handling of structured documents.
This research led to the development of the [BIBLE](/software/bible) system, whose main contribution was the intelligent organization of the various logical and physical representations associated with the processed documents.
The system I developed has set up a form of dynamic sharing based on the delegation and cloning of prototypes.
Its underlying mechanism relied on prototype-based programming, a promising new area of research in the early 1990s  [^Pasquier1992;^Pasquier1994].

## Funding

| Program             | CIFRE Thesis (Conventions Industrielles de Formation par la REcherche)  |
| ------------------- |:----------------------------------------------------------------------- |
| Year                | 1991-1994                                                               |
| Grant recipient     | Claude Pasquier                                                         |
| Funder              | ANRT, on behalf of the French Ministry for Research                     |

## Softwares
* [BIBLE](/software/bible): A system for Design and Management of Context-Controlled Documents

## Related publications
[^Pasquier1992]: {{< cite page="/publication/Pasquier1992" view="4" >}}
[^Pasquier1994]: {{< cite page="/publication/Pasquier1994" view="4" >}}

