+++
# Project title.
title = "2008: mining association rules from gene expression data and annotations."

# Date this page was created.
date = 2019-10-25T00:00:00

# Project summary to display on homepage.
summary = "Software, source files, processed data and results."

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

Martinez, R., Pasquier, N., and Pasquier, C. (2008b), “GenMiner: mining non-redundant association rules from integrated gene expression data and annotations.” Bioinformatics (Oxford, England), Oxford Academic, 24, 2643–4.

### Software ###

The software can be downloaded [here](../../data/bioinformatics_2008/genminer.zip).

### Data sources ###

Gene expression measures are those used by Eisen et al. (Cluster analysis and display of genome-wide expression patterns, PNAS December 8, 1998 vol. 95 no. 25). This dataset is discretized using the NorDi algorithm at a 95% confidence level.

Gene annotations were collected from the following sources:

* **Gene Ontology**: terms were retrieved from [http://archive.geneontology.org](http://archive.geneontology.org), [**local copy of the version of August 2007**](../../data/bioinformatics_2008/go_daily-termdb-data.gz) ; annotations were retrieved from [http://www.geneontology.org](http://www.geneontology.org) [**local copy of the version of August 2007**](../../data/bioinformatics_2008/gene_association.sgd.gz).
* **Literature**: associations between yeast genes and pubmed ids were retrieved from literature curation data at [http://www.yeastgenome.org/](http://www.yeastgenome.org/) [**local copy of the version of August 2007**](../../data/bioinformatics_2008/gene_literature.tab.gz).
* **Patways**: information concerning the metabolic pathways in which each gene is involved was retrieved from [KEGG](http://www.genome.jp/kegg/) [**local copy of the version of August 2007**](../../data/bioinformatics_2008/sce_pathway.list.gz).
* **Phenotype**: annotations were retrieved from [http://www.yeastgenome.org/](http://www.yeastgenome.org/) [**local copy of the version of August 2007**](../../data/bioinformatics_2008/phenotypes.tab.gz).
* **transcriptional regulators**: the information of transcriptional regulators that bind to promoter regions were extracted from [http://younglab.wi.mit.edu/regulatory_network/](http://younglab.wi.mit.edu/regulatory_network/) using a p-value threshold of 0.0005 [**local copy of the version of August 2007**](../../data/bioinformatics_2008/binding_by_gene.tsv.gz).

### Processed Data files ###

#### [**Eisen dataset**](../../data/bioinformatics_2008/EisenYeastData2466-79.txt)
Expression ratios of 2465 Yeast genes under 79 biological conditions.

#### [**Microarray Experiments**](../../data/bioinformatics_2008/EisenYeastData2466-79Cols.txt)
Description of the 79 experiments.

#### [**Cutoffs**](../../data/bioinformatics_2008/EisenYeastData2466-79Intervals.txt)
Under-expressed and over-expressed cutoff thresholds computed by NorDi.

#### [**Discretized expression measures**](../../data/bioinformatics_2008/values.txt)
Discretization of expression measures performed by Nordi.	

#### [**Data mining context**](../../data/bioinformatics_2008/dataset.txt)
Data matrix of 2465 lines (genes) and 737 columns (discretized expression levels and annotations). Each line contains expression profiles over the 79 biological conditions (values discretized by NorDi) and at most 658 gene annotations (24 GOSlim terms, 14 pathways, 25 transcriptional regulators, 14 phenotypes and 581 pubmed IDs).

#### [**Equivalence classes**](../..//data/bioinformatics_2008/fci.zip)
Frequent closed itemsets and their generators extracted by Close with a minsupport of 0.005. Each class if represented by a line of the form

    [Generator] [Closed itemset] n

where 'n' is the number of items in the class.

#### [**Exact associations rules**](../../data/bioinformatics_2008/ear.zip)
All exact association rules displayed in the form

    [antecedent] => [consequent] supp=s conf=c

where 's' and c are the support and the confidence of the rule respectively.

#### [**Approximate associations rules**](../../data/bioinformatics_2008/aar.zip)
All approximate association rules, with a confidence greater or equals to 0.5, displayed in the form

    [antecedent] -> [consequent] supp=s conf=c

where 's' and c are the support and the confidence of the rule respectively
