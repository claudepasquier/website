+++
# Project title.
title = "Generative Programming"

# Date this page was created.
date = 2019-10-24T00:00:00

# Project summary to display on homepage.
summary = "Automatic generation of software tools from specifications."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Software Engineering", "Ended Project"]

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
  caption = "Example of distributed editing."
# that incrementally reflects changes made to the physical view (client side) to the logical view kept on the server side."

  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

#### Active from 2000 to 2002

## Research rationale
Producing high-quality software has become a major concern in industry.
There is a long history of research about providing help and support during the development process.
Generative programming is one of the research areas aimed at improving the quality of software development by offering automatic production of software tools from specifications.

#### A generator of distributed editing tools through the assembly of graphical components

[KeTuK](/software/ketuk) illustrates a way to define editors by assembling graphical components.
A specific layout is obtained by transforming a XML document to be edited into a hierarchy of java components.
The transformation process is made invertible to ensure that any changes to java objects can be reflected in the XML document.
The architecture that has been implemented is open enough to allow the integration of any Java component.

Capitalizing on the work done on KeTuK, we worked on solutions to distribute editing operations over a network.
The adopted principle consists in grouping on a server the XML documents to be edited as well as all the software applications needed for the editing.
The editing operations performed by the clients (who interact on a custom view of the data) are transmitted to the server, which performs the appropriate operations on the central XML document and informs each client of the changes to be reflected in the views.
The data that pass through the network concerns only XML codifications of the operations performed or to be performed.
This system, which limits the necessary code at the client side to the strict minimum, is therefore particularly suitable for editing documents on equipment with limited resources [^Pasquier2000].

#### Automatic generation of softwares from specifications

[SmartTools](http://www-sop.inria.fr/members/Didier.Parigot/SmartTools/) is an ambitious project that aimed to automatically generate development environments from specifications.
The project is strongly based on XML and object technologies and is generic and highly configurable.
In addition to the possibilities of graphical editing on views that can be distributed over a network, SmartTools allows to automatically generate tools (parser, displays, visitors on the document structure) from a language specification.
I participated in the development of SmartTools and ensured the transfer of skills between INRIA's Oasis team and Schlumberger.
In particular, I used the tools provided by the SmartTools software factory to develop an application dedicated to JavaCard operating at the source and bytecode level in an industrial context [^Attali2001a] [^Attali2001b] [^Parigot2002].

## Softwares
* [KeTuK](/software/ketuk): Java based toolkit allowing applications to map XML documents with a set of Java Beans

## Related publications
[^Pasquier2000]: {{< cite page="/publication/Pasquier2000" view="4" >}}
[^Attali2001a]: {{< cite page="/publication/Attali2001a" view="4" >}}
[^Attali2001b]: {{< cite page="/publication/Attali2001b" view="4" >}}
[^Parigot2002]: {{< cite page="/publication/Parigot2002" view="4" >}}
