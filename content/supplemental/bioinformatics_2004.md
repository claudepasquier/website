+++
# Project title.
title = "2004: ontology-driven analysis of microarray data."

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Data sources and processed data files."

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

Pasquier, C., Girardot, F., Jevardat de Fombelle, K., and Christen, R. (2004), *THEA: ontology-driven analysis of microarray data.* Bioinformatics (Oxford, England), Oxford Academic, 20, 2636–43. 


### Data sources ###

Data pre-processing

The CEL files were downloaded from the [Genome-wide Expression Patterns of Drosophila in Response to Immune Challenge Homepage](http://www.fruitfly.org/expression/immunity/) and treated using Bioconductor's affy package (Bioconductor is an open source software that can be dowloaded from [http://www.bioconductor.org/](http://www.bioconductor.org/), the affy package is dedicaced to the analysis of affymetrix data); the releases used were bioconductor 1.2 and affy 1.2.30 (for a review of Bioconductor's specificities, see for example [Dudoit et al., 2003](http://www.ncbi.nlm.nih.gov/pubmed/12664684). The method used to calculate the expression indexes was the 'rma' method, using the default options as described by [Irizarry et al., 2003](http://www.ncbi.nlm.nih.gov/pubmed/12925520) which is arguably one the most pertinent way to process affymetrix arrays measurements so far (for comparisons see [Irizarry et al., 2003](http://www.ncbi.nlm.nih.gov/pubmed/12582260) and [http://affycomp.biostat.jhsph.edu/](http://affycomp.biostat.jhsph.edu/)).

Every possible treated vs control (i.e. infected vs non infected) ratios were computed. These results were subsequently submitted to a SAM multiclass analysis in order to select the genes showing statistically significant variation(s) of expression across experimental conditions (software downloadable from [http://www-stat.stanford.edu/~tibs/SAM/](http://www-stat.stanford.edu/~tibs/SAM/)). The chosen parameters ensured that less than 1% false positives were selected and lead to the selection of 1623 probe-sets of which only those showing a mean fold-change of at least 1.3 in any comparison were retained for further analysis. This further reduced the data to 1290 probe-sets, corresponding to 1277 independent gene products. For each of these selected probe-sets and each experimental conditions the mean of the logged expression values across replicates were calculated, these means where subsequently used to calculate the different infected/uninfected logged expression ratios. This dataset was then uploaded on the bioinformatics web site of CNIO (http://bioinfo.cnio.es) [Herrero et al., 2003](http://www.ncbi.nlm.nih.gov/pubmed/12824345)), where the use of a preprocessor [Herrero et al., 2003](http://www.ncbi.nlm.nih.gov/pubmed/12651726) allowed the merging of the replicates (using the median of the ratios) as well as the generation of various entry files for the different classification programs available on the same server. We chose to realize a SOTA analysis [Herrero et al., 2001](http://www.ncbi.nlm.nih.gov/pubmed/?term=11238068) using the 'correlation coefficient (linear)' metrics and '90% variability' as end training condition. The generated tree was loaded in THEA and analyzed using the program's features.

### Processed Data files ###

#### [**RMA data**](../../data/bioinformatics_2004/DeGregorio_RMA_data.txt)
Expression levels calculated with the RMA method.	

#### [**expression ratios**](../../data/bioinformatics_2004/DeGregorio_RMA_SAM_FC_data_moy_ratios_GEPASmerged.sdt)
Infected/uninfected logged expression ratios of the replicates merged by GEPAS (using the median of the ratios).

#### [**SOTA tree**](../../data/bioinformatics_2004/DeGregorio_RMA_SAM_FC_data_moy_ratios_GEPASmerged.sot)
Result of the SOTA analysis (Herrero et al., 2001) using the 'correlation coefficient (linear)' metrics and '90% variability' as end training condition.	

#### [**Table_S1**](../../data/bioinformatics_2004/Table_S1.rtf)
Statistics of the namings realized by THEA using the cutoffs described in the legend of the Figure 3 of the paper. (MF: Molecular Fonction, CC: Cellular Component, BF: Biological Fonction, DGA: Drosphila Gross Anatomy, DDS : Drosophila Developmental Stage).	

#### [**Table_S2**](../../data/bioinformatics_2004/Table_S1.rtf)
Comparison of THEA and other related programs.


