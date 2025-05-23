+++
# Project title.
title = "KeTuK"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Mapping XML documents with a set of Java Beans."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Software Engineering", "XML Documents Editing"]

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
links = [{name="Go to Project Site", url = "http://www-sop.inria.fr/lemme/Claude.Pasquier/ketuk/"}, {name="Get Source Code", url="data/KeTuK.zip"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Dependency graph of the sentence '*mir1 inhibits gastric cancer cell proliferation and migration by targeting MET*'"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

| KeTuK          |              |
| -------------- | ------------ |
| Release date   | 2000         |
| Implementation | Java         |
| Author         | Pasquier, C. |

KeTuK [^Pasquier2000] is a Java based toolkit allowing applications to map XML documents
with a set of Java Beans. The idea is to use Java Beans as an interface
for XML documents. Depending on the behaviour of the Java Beans used,
various operations, ranging from visualization to edition or generation
can be performed. An overview of the application is proposed [here](http://www-sop.inria.fr/lemme/Claude.Pasquier/ketuk/overview.html).

#### Getting started

KeTuK use [XSLT](http://www.w3.org/TR/xslt.html) to express the mapping
between XML and Java Beans. Users not familiar with XSLT should have a
look at the W3C Recommendation on Java Beans..

From this point, the [KeTuK's Tutorial](http://www-sop.inria.fr/lemme/Claude.Pasquier/ketuk/tutorial.html) show that writing
an KeTuK description to define an editor is as simple as writing an XSLT
description to produce HTML. It shows several snapshots of the resulting
Java Beans interface. A more exhaustive documentation is proposed
[here](http://www-sop.inria.fr/lemme/Claude.Pasquier/ketuk/documentation.html). Some [samples](http://www-sop.inria.fr/lemme/Claude.Pasquier/ketuk/samples.html) are included in the KetUk package.

#### KeTuK availability

KeTuK is written in pure Java and works on all releases of Java 2. It is
available in both source code and precompiled binary (JAR files) form.
Both KeTuK packages are made available under the LGPL Software License.

#### Resources

KeTuK makes use the following softwares:

-   [Java MultiMethod
    Framework](http://igm.univ-mlv.fr/~forax/works/jmmf/index.html)
    implementing multi-polymorphism in java,
-   [Xerces](http://xml.apache.org/xerces-j/index.html), a XML parser in
    Java,
-   [Xalan](http://xml.apache.org/xalan-j/index.html), a XSLT stylesheet
    processors in Java,
-   [Ant](http://jakarta.apache.org/ant/index.html), a Java based build
    tool.

The beans used in the demos are based on the graphical swing-based
components developed in Kuil.

#### Related publication
[^Pasquier2000]: {{< cite page="/publication/Pasquier2000" view="4" >}}


