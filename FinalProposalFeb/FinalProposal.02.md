Initial Proposal
================
**Gene Machine**
Feb 13th 2019

Title of project
----------------

This is initial proposal for **Team Gene Machine**.

Our team members are:

<table style="width:32%;">
<colgroup>
<col width="13%" />
<col width="18%" />
</colgroup>
<thead>
<tr class="header">
<th>Github ID</th>
<th>Name</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span class="citation">[@garyzhubc]</span>(<a href="https://github.com/garyzhubc" class="uri">https://github.com/garyzhubc</a>)</td>
<td>Gary / Peiyuan Zhu (MSc, Statistics)</td>
</tr>
<tr class="even">
<td><span class="citation">[@glenn-mcguinness]</span>(<a href="https://github.com/glenn-mcguinness" class="uri">https://github.com/glenn-mcguinness</a>)</td>
<td>Glenn McGuinness (MSc, Statistics)</td>
</tr>
<tr class="odd">
<td><span class="citation">[@janxue]</span>(<a href="https://github.com/janxue" class="uri">https://github.com/janxue</a>)</td>
<td>Jan Xue (MSc, Botany)</td>
</tr>
<tr class="even">
<td><span class="citation">[@j-schaub]</span>(<a href="https://github.com/j-schaub" class="uri">https://github.com/j-schaub</a>)</td>
<td>Jessica Schaub (MSc, Oceanography)</td>
</tr>
<tr class="odd">
<td><span class="citation">[@ymkng]</span>(<a href="https://github.com/ymkng" class="uri">https://github.com/ymkng</a>)</td>
<td>Michelle Kang (MSc, Bioinformatics)</td>
</tr>
</tbody>
</table>

*Our project is based on there data from:*

-   [GSE20586](https://bit.ly/2UEOxqj) from the paper [Arabidopsis VASCULAR-RELATED NAC-DOMAIN6 Directly Regulates the Genes That Govern Programmed Cell Death and Secondary Wall Formation during Xylem Differentiation](https://bit.ly/2WJtnJI)

-   [GSE77153](https://bit.ly/2t3Egbv) from the paper [A Transcriptional and Metabolic Framework for Secondary Wall Formation in Arabidopsis](https://bit.ly/2Txs0vk).

Proposal
--------

The following proposal is meant to give an outline of our project with an introduction, objectives, description of the data, proposed major analysis, and a breakdown of assigned tasks.

### Abstract

The plant cell wall determines cell shape, rigidity, and architecture ultimately affecting the mechanical strength of the tissues. There are two general types of cell walls, primary cell walls, formed and modified in growing cells, and secondary cell walls, laid down after the cell has stopped growing in some cell types as a process of cell differentiation influencing both mechanical strength and permeability to water. In particular a majority of secondary cell walls are found in cells specialized in conducting fluids, such as water transportation. A common example of highly visible secondary cell walls is wood, where the cells have died but the secondary cell wall remains. More specifically, metaxylem, protoxylem, and interfasicular fibers are water conducting cell types with secondary cell walls that are commonly studied in arabidopsis (figure 1).

![Differentiation of pre xylem cells](https://bit.ly/2Bo7QNr)

Figure 1. Focusing on the left side of this diagram, illustration of undifferentiated parenchymatous plant cells into the various xylem cell types : protoxylem, metaxylem, and fibres. This figure is from Schuetz et al. 2012.

The production of these secondary cell walls involves a tightly regulated transcriptional network. Specifically 5 transcription factors (SND1, VND7, VND6, NST1, and NST2) have been characterized as "master transcription factors" capable of activating the entire secondary cell wall biosynthetic program. For example when VND7 is activated, it is able to turn on the helical pattern of secondary cell wall formation. For a more detailed schematic describe some overall regulatory pathways of secondary cell wall synthesis see [here](https://bit.ly/2RDoEFt).

![helical pattern of secondary cell wall formation](https://bit.ly/2GbXSTv)

Figure 2. Induced VND7 turns on secondary cell wall formation in BY2 cells. Normally BY2 cells would not produce secondary cell walls.

Despite all controlling secondary cell wall formation, the cell type and resulting secondary cell wall composition and shape differ based on the transcription factor turned on. VND7, VND6 and SND1 are thought to turn on secondary cell wall formation in metaxylem, protoxylem, and fiber cell types respectively but are generally all expressed to a certain degree during secondary cell wall formation (Kubo et al., 2005; Zhong, Demura, & Ye, 2006). However, the secondary cell walls in these cell types are markedly different as can be seen in figure 2., protoxylem with the helical, metaxylem with reticulate, or fibers with thick evenly distributed secondary cell wall thickenings, and the global underlying expressional differences regulating this morphological differentiation remains elusive.

There have been some studies that have looked into the differential expression patterns induced after turning on the master transcription factors of secondary cell wall biosynthesis. For example, Ito et al. (2010) have demonstrated that VND6 and SND1 each regulated a small non-overlapping fraction of genes with distinct biological roles of programmed cell death or monolignol (a polymer specific to the secondary cell wall) biosynthesis (Ohashi-Ito, Oda, & Fukuda, 2010). They did this by turning on the expression of SND1 in suspended Arabidopsis cells and measuring expression at 0 hours and 12hours, i.e. before and as secondary cell wall is being formed. They then repeated this with VND6. Moreover, another study by Li et al. (2016) looked at VND7 seedlings and turned on their expression measuring again at 0 and 12hours respectively (Li et al., 2016). Both of these studies used commercial affametrix arrays for Arabidopsis. More information on the \[ATH1-121501\] Affymetrix Arabidopsis ATH1 Genome Array used can be found [here](https://bit.ly/2MN380j).

The differentiation of xylem precursors into protoxylem and metaxylem are markedly different (as depicted in figure 1) and as a result, one would imagine that transcriptional regulation by either VND6 or VND7 would yield overlapping but differential gene regulation. To date, no one has explicitly compared these particular differences on a global scale. As a result, we would like to try and compare????

-   DE expression analysis
-   Combining data
-   Give GO annotations
-   For DE genes look for TEREs
-   Network analysis

### Motivation

[paper](link) demonstrate that:

-   a
-   b

[paper](link) demonstrate that:

-   a
-   b

### Goals

based on the data collected from Li et al. 2018, we will :

1.Given the expression level of genes in tissues expressing VND6 or VND7 or SND1, determine if the gene is differentially expressed in VND6 or VND7 or SND1.

1.  Reconfirm their results by trying to reproduce their (1) clustering analysis of the RNA- seq data between the groups of parents and offpring that the authors have already defined, (2) their differential expression analysis to see if we obtain the same differentially expressed genes that they did wioth visualization through a heat map and dendrogram

2.  Do the differentially expressed genes in the hybrid offspring also correlate with close by methylation differences. To visualize this we will compare the differences in methylation amongst differentially expressed genes in a scatter plot. Moreover, Li et al 2018 distiguish the methylation sites into 2 different data sets, methylated and hypomethylated.

3.  Do we consider the expression or methylation data different between the sets of parents. WHat about the offspring. In order to address this we can inlcude parents and offspring as a factor and test if they are distinct groups through **statical means**.

*We can find genes that were differentially expressed between parents and offspring.Instead of treating them sepparately, we will try pooling the parents and pooling the offspring data. &lt; unsure about this&gt;*

### Description of Data

the data provided from Li et al. 2018 paper :

-   RNA seq data with x. the samples included are :

-   Raw methylation dat with number of counts
-   sample description here

### Methods and Division of Labour

-   Test whether the parental lines more simmilar to each other than to the offspring with regards to the expression data? how about the methylation data? (cluster analysis)
-   Find differentially expressed genes with two approaches. First try between each parent child triad. Then try again by pooling the parental data and pooling the child data. How different are these results?

### Works cited

Kubo, M., Udagawa, M., Nishikubo, N., Horiguchi, G., Yamaguchi, M., Ito, J., … Demura, T. (2005). Transcription switches for protoxylem and metaxylem vessel formation. Genes & Development, 19(16), 1855–1860. <https://doi.org/10.1101/gad.1331305>

Li, Z., Omranian, N., Neumetzler, L., Wang, T., Herter, T., Usadel, B., … Persson, S. (2016). A Transcriptional and Metabolic Framework for Secondary Wall Formation in Arabidopsis. Plant Physiology, 172(2), 1334–1351. <https://doi.org/10.1104/pp.16.01100>

Ohashi-Ito, K., Oda, Y., & Fukuda, H. (2010). &lt;em&gt;Arabidopsis&lt;/em&gt; VASCULAR-RELATED NAC-DOMAIN6 Directly Regulates the Genes That Govern Programmed Cell Death and Secondary Wall Formation during Xylem Differentiation. The Plant Cell, 22(10), 3461 LP-3473. <https://doi.org/10.1105/tpc.110.075036>

Zhong, R., Demura, T., & Ye, Z.-H. (2006). SND1, a NAC Domain Transcription Factor, Is a Key Regulator of Secondary Wall Synthesis in Fibers of &lt;em&gt;Arabidopsis&lt;/em&gt; The Plant Cell, 18(11), 3158 LP-3170. <https://doi.org/10.1105/tpc.106.047399>