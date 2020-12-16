+++
# Project title.
title = "Attributed Graph Mining"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Combining itemset mining and structural mining to reveal patterns in attributed graphs."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Attributed Graph Mining", "Graph Mining", "Ended Project"]

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
#url_slides = "data/slides.pdf"
url_video = ""
url_code = ""

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
#links = [{icon_pack = "fab", icon="twitter", name="Follow", url = "https://twitter.com/georgecushen"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Illustration of the possible extensions of a pattern with automorphisms."
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
#markup: mmark

+++

#### Active from 2012 to 2014

[//]: # (This may be the most platform independent comment)

## Research rationale
Graphs are well suited to model complex structures present in the real world.
Because of this ubiquitousness, graphs are extensively studied in graph theory, and, more recently, in the field of data mining.
Until the 2000s, most research focused either on unlabeled graphs or on graphs with nodes associated with a single label.
However, in many applications, objects (represented by nodes) are associated with multiple characteristics, and these can be represented as node attributes.
Graphs in which nodes are annotated with sets of attributes (or itemsets) are named attributed graphs and up to now, only few studies are devoted to their analysis.

Mining attributed graphs is very difficult because the search space is much larger than for labeled graphs.
However, there is a need for effective methods that can help identify hidden structural patterns, but which can also highlight the relationship between node attributes.

## Results

#### A new mining algorithm combining itemset extension and structural extension
The strategy for searching for frequent patterns that we have proposed is to start from a set of initial patterns composed of nodes associated with a single item and to build the search tree from the spanning tree originating from these nodes, using an order based on a code that we have defined.
We proposed a complete method for navigating the search space that combines two extension types: itemset extension and structure extension.
We empirically defined the notion of closure on attributed graphs by considering that an attributed graph is closed if it is not included in any other attributed graph that has the same support as it.
We have also proposed two concise representations of the patterns that are defined either according to the inclusion on itemsets (c-closed patterns), or according to the inclusion on the structures (s-closed patterns).
We have shown that the enumeration of c-closed patterns allows to drastically reduce both the number of returned patterns and the execution time.
Tests have shown that this condensed representation offers a good compromise between speed of execution and conciseness of results[^Pasquier2013a;^Pasquier2013b;^Pasquier2016b].

#### Handling of cycles and isomorphic patterns
The consideration of cycles in a graph required a special treatment of the isomorphic patterns that are inevitably generated for all explorations that start on another node that is part of the cycle.
Patterns that have many subgraph isomorphisms with the analyzed pattern present difficulties for all existing algorithms because the problem of subgraph isomorphisms is NP-complete.
We have proposed two optimizations that make it possible, on the one hand, to trim the search tree generated from an automorphic pattern and, on the other hand, to delete certain ways of obtaining automorphic patterns that do not allow new canonical patterns to be generated [^Pasquier2014b;^Pasquier2017b].

#### A new condensed representation of weighted paths
We have addressed the problem of extracting frequent weighted paths in a single attributed directed acyclic graph (aDAG) where each weight expresses the frequency of a transition.
Frequent paths are used to analyze the causal relationship between sequences of events and/or attributes.
As the number of patterns can be very large, we have designed a condensed representation for such collections[^Sanhes2013a;^Sanhes2013b].

#### Integrating mathematical models defined by experts into the extraction process 
By noting that in many data science contexts, experts have often capitalized part of their knowledge in mathematical models, we have proposed to use these models to derive new constraints that can be used during the data mining phase to improve both pattern relevancy and computational efficiency 
We have defined a method of patterns mining under constraint of a modele. 
We also studied some properties of predicates and constraints in order to use them to optimize pattern calculations.
We have shown that taking into account constraints from mathematical models makes it possible to better target analysis, while improving performance through model properties.
We have thus obtained more relevant patterns, complementing or contradicting the expert knowledge on the studied phenomena [^Flouvat2014a;^Flouvat2014b].

## Funding

| Program             | ANR Program FOSTER                             |
| ------------------- |:----------------------------------------------------------------------- |
| Year                | 2011-2013                                                               |
| Funder              | ANR                                       |
| Grant name          | Spatio-temporal data mining: application to the understanding and monitoring of soil erosion |
| Grant id            | ANR-10-COSI-012
| Project coordinator | Nazha-Selmaoui Folcher                                                           |

## Softwares
* [AADAGE](/software/aadage): Extraction of frequent patterns in attributed graphs
* [IMIT](/software/imit): Mining frequent patterns in attributed trees

## Related publications
[^Pasquier2013a]: {{< cite page="/publication/Pasquier2013a" view="4" >}}
[^Pasquier2013b]: {{< cite page="/publication/Pasquier2013b" view="4" >}}
[^Pasquier2016b]: {{< cite page="/publication/Pasquier2016b" view="4" >}}
[^Pasquier2014b]: {{< cite page="/publication/Pasquier2014b" view="4" >}}
[^Pasquier2017b]: {{< cite page="/publication/Pasquier2017b" view="4" >}}
[^Sanhes2013a]: {{< cite page="/publication/Sanhes2013a" view="4" >}}
[^Sanhes2013b]: {{< cite page="/publication/Sanhes2013b" view="4" >}}
[^Flouvat2014a]: {{< cite page="/publication/Flouvat2014a" view="4" >}}
[^Flouvat2014b]: {{< cite page="/publication/Flouvat2014b" view="4" >}}

