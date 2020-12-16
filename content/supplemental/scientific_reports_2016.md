+++
# Project title.
title = "2016: predicting miRNA-disease associations with a vector space model."

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Data sources and results (Supplementary Table S1 to S6)."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
#tags = ["Attributed Graph Mining", "Graph Mining", "Ended Project"]

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
  caption = "Illustration of the possible extensions of a pattern with automorphisms."
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
#markup: mmark

+++

### Data associated with the article:

Pasquier, C., and Gardès, J. (2016), *Prediction of miRNA-disease associations with a vector space model.* Scientific reports, Nature Publishing Group, 6, 27036.

### Data sources ###

The method is based on the analysis of the following ressources:

* experimentally verified miRNA-disease associations retrieved from [human miRNA-disease database (HMDD) v2.0](http://www.cuilab.cn/hmdd) [1]
* standard disease names included in the [Medical Subject Headings (MeSH) terms](https://www.ncbi.nlm.nih.gov/mesh)
* experimentally validated miRNA-mRNA interaction, downloaded from [miRTarBase](http://mirtarbase.mbc.nctu.edu.tw/) [2]
* family, genomic location and textual description of miRNAs stored in [miRBase](http://www.mirbase.org/) [3]
* abstract of research papers associated with every miRNA stored in miRBase retrieved from [Pubmed](https://www.ncbi.nlm.nih.gov/pubmed)

### Results ###
* [Supplementary Table S1](../../data/mirai_2016/Suppl_Table_S1.xls) Average AUC obtained on 83 diseases
* [Supplementary Table S2](../../data/mirai_2016/Suppl_Table_S2.xls) list of 86 associations included in HMDD that obtain a significant score of invalidation
* [Supplementary Table S3](../../data/mirai_2016/Suppl_Table_S3.xls) AUC scores obtained for the 15 important diseases using the updated database
* [Supplementary Table S4](../../data/mirai_2016/Suppl_Table_S4.xls) AUC scores obtained for all the diseases using the revised reference database
* [Supplementary Table S5](../../data/mirai_2016/Suppl_Table_S5.xls) List of 126 potential new associations between miRNAs and diseases identified by MiRAI using the revised reference database (confirmed associations are highlighted in green)
* [Supplementary Table S6](../../data/mirai_2016/Suppl_Table_S6.xls) List of 72 putative new associations that need to be confirmed

### Generated data ###
* [mirna_descriptions.zip](../../data/mirai_2016/mirna_descriptions.zip) miRna descriptions specified in MirBase
* [mirna_mirbase_abstracts.zip](../../data/mirai_2016/mirna_mirbase_abstracts.zip) abstracts of PubMed articles associated with miRNAs in MirBase
* [mirna_abstracts.zip](../../data/mirai_2016/mirna_abstracts.zip) abstracts of PubMed articles associated with miRNAs (automatically retrieved by parsing the abstracts)
* **[Updated Reference database](../../data/mirai_2016/miRNA_disease.xls)** The manually curated database of miRNA-disease associations, obtained as described in the paper

### References ###
[1] Li, Y. et al. HMDD v2.0: A database for experimentally supported human microRNA and disease associations. Nucleic
Acids Res. 42, 1070–1074 (2014).

[2] Hsu, S. D. et al. MiRTarBase: A database curates experimentally validated microRNA-target interactions. Nucleic Acids Research 39, 163–169 (2011).

[3] Griffiths-Jones, S., Grocock, R. J., van Dongen, S., Bateman, A. & Enright, A. J. miRBase: microRNA sequences, targets and gene
nomenclature. Nucleic acids research 34, D140–D144 (2006).

