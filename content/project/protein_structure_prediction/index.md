+++
# Project title.
title = "Protein Structure Prediction"

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Prediction of localization and topology of transmembrane alpha-helices in proteins."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Computational Biology", "Ended Project"]

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
  caption = "Example of predicted transmembrane segment topologies for three proteins."
# that incrementally reflects changes made to the physical view (client side) to the logical view kept on the server side."

  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

#### Active from 1997 to 1999

## Research rationale
Membrane proteins are involved in a wide range of essential functions, including the communication between cells and the transport of nutrients, ions, and waste products across biological membranes.
These proteins, that are estimated to constitute 25% of proteins at a genomic scale, play key roles in an equally wide range of diseases like diabete, hypertension, depression, arthritis and cancer.
They are also common drug targets (for over 75% of pharmaceuticals in use today).
Determining membrane protein structures is essential for the understanding of how drugs interfere with cellular communication and regulation.
However, current knowledge about the detailed 3D structures of membrane proteins is limited, because such protein structures are difficult to study by traditional experimental methods.

The idea is to use computational techniques to enhance our knowledge about membrane proteins.
However, developing algorithms that are capable of predicting the three-dimensional structure of proteins at atomic detail is a very difficult task.
Instead of tertiary structure determination, we focused our research on two complementary aspects: **the structural classification of proteins**, which allows to identify potential membrane proteins, and **the prediction of transmembrane alpha-helices in membrane proteins.**

## Results

#### Structural classification of proteins
Periodical patterns and tandem repeats of residues are often found in DNA and protein sequences.
In proteins, their presence helps towards an understanding of the molecular structure of a fibrous/structural protein employing the principle of conformational equivalence and it may suggest ways of ultramolecular assembly for the formation of higher order structure.
Characteristic examples are periodicities found in a number of sequences of fibrous proteins (e.g. tropomyosin, myosin, keratins and collagen).
We used the Fourier analysis method to highlight hidden periodicities in protein sequences and developped [FT](/software/ft), a tool accessible by biologists through the Internet[^Pasquier1998a] [^Pasquier1998b].

In the continuation of this work, we explored the use of hierarchical, artificial neural networks for the generalized classification of proteins into several distinct classes - transmembrane, fibrous, globular, and mixed - from information solely encoded in their amino
acid sequences [^Pasquier1999c] [^Pasquier2001] [^Promponas2001].
The use of our implementations ([PRED-TMR2](/software/pred-tmr2) and [PRED-CLASS](/software/pred-class)) to analyze various test sets and complete proteomes of several organisms demonstrates that such methods could serve as a valuable tool in the annotation of genomic open reading frames with no functional assignment or as a preliminary step in fold recognition and ab initio structure prediction methods [^Promponas1998] [^Promponas1999] [^Pasquier1999b] [^Liakopoulos2000] [^Liakopoulos2001b] [^Iliopoulos2003].

#### Prediction of transmembrane alpha-helices in membrane proteins

The successful location of transmembrane segments, of their secondary structure and the packing modes of secondary structure elements is important because they define the architecture of a transmembrane protein.
However, equally important is the determination of topology, which defines the polarity of integral membrane proteins.

Researchers have identified several characteristics that are common to a large proportion of transmembrane segments.
They observed, for example, that transmembrane segments are mainly composed of hydrophobic residues, and that the propensity of positively charged residues is higher in the non-transmembrane segments on the inner part of the cell, also that a high propensity of tyrosine and tryptophan indicates the outer part of the cell.
To enhance this knowledge, we performed several statistical analysis of known transmembrane segments to find other characteristics of transmembrane parts.
We determined, among other things, the distribution of transmembrane segment length, the propensity for each amino acid to be in a transmembrane region and the precise profiles of potential termini ("edges", starts and ends) of transmembrane regions [@Pasquier1999a].
We combined this information with several scoring functions to predict the precise position of transmembrane segments and their topology [^Liakopoulos1999] [^Liakopoulos2001a].
The accuracy of our method compares well with that of other popular existing methods.
This work led to the implementation of several tools freely available on the Internet: [PRED-TMR](/software/pred-tmr), [OrienTM](/software/orientm), [CoPreTHi](/software/coprethi) and [Dam-Bio](/software/dam-bio).

## Funding
| Program             | Training and Mobility of Researchers (TMR)                              |
| ------------------- |:----------------------------------------------------------------------- |
| Year                | 1997-1999                                                               |
| Funder              | European Economic Community (EEC)                                       |
| Grant name          | EEC-TMR "GENEQUIZ", Integrated Software System for Molecular Biologists |
| Grant id            | ERBFMRXCT960019                                                         |
| Project coordinator | Chris Sanders                                                           |

## Softwares
* [COPRETHI](/software/coprethi): Ensemble learning to predict transmembrane segments in proteins
* [DAM-BIO](/software/dam-bio): Integrated environment designed to support protein sequence and structure analysis on the Web
* [DB-NTMR](/software/db-ntmr): Database of non transmembrane regions automatically extracted from the SwissProt database
* [DB-TMR](/software/db-tmr): Database of transmembrane regions automatically extracted from the SwissProt database
* [FT](/software/ft): Analysis of periodic patterns in amino acid or DNA sequences by Fourrier transform
* [ORIENTM](/software/orientm): Topology prediction of transmembrane proteins and segments
* [PRED-CLASS](/software/pred-class): System of cascading neural networks that classifies any protein into one of four possible classes: membrane, globular, fibrous, mixed
* [PRED-TMR](/software/pred-tmr): Prediction of transmembrane domains in proteins
* [PRED-TMR2](/software/pred-tmr2): Identification of transmembrane proteins and prediction of their transmembranle domains

## Related publications
[^Pasquier1998a]: {{< cite page="/publication/Pasquier1998a" view="4" >}}
[^Pasquier1998b]: {{< cite page="/publication/Pasquier1998b" view="4" >}}
[^Pasquier1999c]: {{< cite page="/publication/Pasquier1999c" view="4" >}}
[^Pasquier2001]: {{< cite page="/publication/Pasquier2001" view="4" >}}
[^Promponas2001]: {{< cite page="/publication/Promponas2001" view="4" >}}
[^Promponas1998]: {{< cite page="/publication/Promponas1998" view="4" >}}
[^Promponas1999]: {{< cite page="/publication/Promponas1999" view="4" >}}
[^Pasquier1999b]: {{< cite page="/publication/Pasquier1999b" view="4" >}}
[^Liakopoulos2000]: {{< cite page="/publication/Liakopoulos2000" view="4" >}}
[^Liakopoulos2001b]: {{< cite page="/publication/Liakopoulos2001b" view="4" >}}
[^Iliopoulos2003]: {{< cite page="/publication/Iliopoulos2003" view="4" >}}
[^Liakopoulos1999]: {{< cite page="/publication/Liakopoulos1999" view="4" >}}
[^Liakopoulos2001a]: {{< cite page="/publication/Liakopoulos2001a" view="4" >}}

