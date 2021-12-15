+++
# Project title.
title = "Omics Data Mining"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Semantic integration and analysis of biological data."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Computational Biology", "Active Project"]

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
  caption = "Overview of our analysis pipeline."
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

#### Active since 2000

## Research rationale
In the late 1990s, new techniques for measuring the expression of genes at the level of entire genomes have emerged.
By combining these quantitative measurements with biological knowledge, this breakthrough has paved the way for deciphering the activity of genes, their interactions and their involvement in various biological processes.
However, the analysis of this mass of data remained a manual task.
Firstly, because, although there were many different sources storing biological data, all these sources were completely independent of each other, and secondly, because tools to analyse these data in an automated way did not yet exist.
Solutions to integrate heterogeneous data and to automate their analysis were more than ever needed.

## Results

#### A methodology to ease data integration using Semantic Web technologies
Our research started with the idea that Semantic Web technologies, which provide a common framework allowing data to be shared and reused between applications, might be applied to the management of disseminated biological data.
We studied and reported the specificities of biological data that made the application of these technologies to the life sciences a real challenge.
Then, we proposed a methodology to facilitate data integration using Semantic Web whose precepts were very close to the rules that currently govern the Web of Data [^Pasquier2008a] [^Pasquier2011].
We implemented our ideas in [AllOnto](/software/allonto), a Knowledge Base System capable of storing and performing queries on large sets of RDF/OWL specifications (including the storing and querying of reified statements).
The software was designed to handle the provenance of information and included reasoning capabilities dealing with type inference, transitivity and built-in OWL constructs like *owl:sameAs* and *owl:inverseOf*.

Allonto was applied to collect and integrate data used in three different approaches of data mining we investigated.

#### Automatic gene annotation through a data-driven approach
The data-driven approach involves first identifying groups of genes whose expression shows similar variation and then integrating knowledge about genes.
The research on this topic took the form of an integrated system called [THEA](/software/thea) (Tools for High-throughput Experiments Analysis).
The software integrates several data mining algorithms to automatically annotate groups of genes sharing similar expression profiles with biological information (various ontologies, chromosomal localization, link with diseases).
Experiments show that using THEA not only makes it easy and quick to obtain all manually highlighted results, but also to pinpoint new findings [^Pasquier2004a] [^Pasquier2004b].

#### Automatic gene annotation through a knowledge-driven approach
The knowledge-driven approach consists of first finding co-annotated groups of genes and then, in a second step, integrating data on expression profiles.
The [CGGA](/software/cgga) method (Co-expressed Gene Groups Analysis), which we developed, is part of this approach.
The tests that have been carried out show that the functional annotations provided by CGGA reduce the complexity of the data analysis problem by integrating various types of information about genes.
The experimental results showed the interest of the approach and made it possible to identify relevant information on the biological processes studied [^Martinez2005] [^Martinez2006a] [^Martinez2006c] [^Martinez2008c] [^Pasquier2008b] [^Martinez2009].

#### Extraction of association rules from a heterogeneous set of gene data
We have proposed the use of Association Rule Discovery (ARD) as a method capable of identifying rules linking any pieces of biological data and which does not impose any ordering over the use of data sources.
We developed an application called [GenMiner](/software/genminer) to fully exploit the capacities of ARD in the context of biological data mining.
GenMiner allows the joint use of knownledge about genes and their level of expression under certain conditions in order to discover the relationships between a priori knowledge and experimental measurements.
Our method includes a new algorithm, called [NorDI](/software/nordi) (Normal DIscretization algorithm) to discretize gene expression measurements and generate expression profiles.
The experiments we conducted confirmed the advantages of GenMiner over known approaches.
GenMiner allows to search for association rules using a much smaller minimum support than what is possible with traditional approaches.
In addition, GenMiner significantly reduces the number of extracted rules, making it much easier for the end user to explore and interpret [^Martinez2007] [^Martinez2008a] [^Martinez2008b].

Alongside these activities, research was also carried out on the parallelization of the Blast algorithm [^Anand2004].
Collaborations with biologists still continue, resulting in collaborative research where we are primarily responsible for data analysis [^Pasquier2014a].

## Funding

| Program             | Inter-EPST Program on bioinformatics                              |
| ------------------- |:----------------------------------------------------------------------- |
| Year                | 2002-2004                                                               |
| Funder              | CNRS, INSERM, INRA, INRIA, Ministry of Research                                       |
| Grant name          | The use of a knowledge base system to analyze microarray data |
| Project coordinator | Claude Pasquier                                                           |

| Program             | CNRS Bio-STIC-LR                              |
| ------------------- |:----------------------------------------------------------------------- |
| Year                | 2005-2007                                                               |
| Funder              | CNRS, INSERM, INRA, INRIA, Ministry of Research                                       |
| Grant name          | Towards an editor for the subdivision of trees into sub-trees collections formals and functionals criteria for the subdivision process, intra-inter collection trees comparaisons |
| Project coordinator | François Chevenet                                                           |

| Program             | CNRS post-doctoral grant                              |
| ------------------- |:----------------------------------------------------------------------- |
| Year                | 2008-2010                                                               |
| Funder              | CNRS                                       |
| Grant name          | Transcriptome mass data use and interpretation using the Massively Parallel Signature Sequencing (MPSS) technologies |
| Grant recipient     | Ronnie Alves |
| Project coordinator | Claude Pasquier                                                           |

| Program             | ANR Methylclonome                              |
| ------------------- |:----------------------------------------------------------------------- |
| Year                | 2013-2015                                                               |
| Funder              | ANR                                       |
| Grant name          | Analyse de l’héritabilité des traces épigénétiques dans la reproduction clonale |
| Grant id     | ANR-12-BSV6-0006 |
| Project coordinator | Alain Robichon                                                           |

| Program             | Gliosplice                             |
| ------------------- |:----------------------------------------------------------------------- |
| Year                | 2017-2020                                                               |
| Funder              | Institut National du Cancer (INCa)                                        |
| Grant name          | Characterization of alternative splicing networks coordinating brain tumor heterogeneity and treatment resistance commitment |
| Project coordinator | Mathieu Gabut                                                           |

## Softwares
* [AllOnto](/software/allonto): Knowledge Base System to store and query RDF/OWL specifications
* [CGGA](/software/cgga): Extraction of bi-clusters of genes
* [GenMiner](/software/genminer): Mining equivalence classes and minimal non-redundant association rule from gene expression data
* [NORDI](/software/nordi): Discretization of gene expression data according to the distribution of the dataset
* [THEA](/software/thea): Integrated information processing system dedicated to the annotation of transcriptomic results
* [Thea-Interact](/software/thea-interact): Analysis of the interaction network of Drosophila genes
* [Thea-Online](/software/thea-online): Web portal using Semantic Web technologies to integrate, query and display information from multiple sources


## Related publications
[^Pasquier2008a]: {{< cite page="/publication/Pasquier2008a" view="4" >}}
[^Pasquier2011]: {{< cite page="/publication/Pasquier2011" view="4" >}}
[^Pasquier2004a]: {{< cite page="/publication/Pasquier2004a" view="4" >}}
[^Pasquier2004b]: {{< cite page="/publication/Pasquier2004b" view="4" >}}
[^Martinez2005]: {{< cite page="/publication/Martinez2005" view="4" >}}
[^Martinez2006a]: {{< cite page="/publication/Martinez2006a" view="4" >}}
[^Martinez2006b]: {{< cite page="/publication/Martinez2006b" view="4" >}}
[^Martinez2006c]: {{< cite page="/publication/Martinez2006c" view="4" >}}
[^Martinez2008c]: {{< cite page="/publication/Martinez2008c" view="4" >}}
[^Pasquier2008b]: {{< cite page="/publication/Pasquier2008b" view="4" >}}
[^Martinez2009]: {{< cite page="/publication/Martinez2009" view="4" >}}
[^Martinez2007]: {{< cite page="/publication/Martinez2007" view="4" >}}
[^Martinez2008a]: {{< cite page="/publication/Martinez2008a" view="4" >}}
[^Martinez2008b]: {{< cite page="/publication/Martinez2008b" view="4" >}}
[^Anand2004]: {{< cite page="/publication/Anand2004" view="4" >}}
[^Pasquier2014a]: {{< cite page="/publication/Pasquier2014a" view="4" >}}

