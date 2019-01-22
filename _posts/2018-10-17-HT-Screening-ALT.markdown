---
layout: post
title:  "High-Throughput Screening for ALT Genes"
date:   2017-10-17 22:42:40 -0700
categories: ALT Biology
---

Note: This is a grant application that I co-authored with my research mentor HS.

## Abstract
There are many proposed methods to inhibit growth of various types of cancer, but none are as
universal as abrogating telomere maintenance mechanisms (TMMs). Telomerase has been widely
studied for decades as a cancer target and as such telomerase-based anti-cancer strategies have
received extensive support from academia and industry. High throughput telomerase-based assays have
been extensively used to discover and develop various telomerase inhibitors that are now being tested
in clinical trials. However, a significant portion of cancer uses a telomerase-independent mechanism
known as ALT, and recent reports suggest that some tumors may activate both TMMs simultaneously
and that telomerase inhibition may select for ALT cancer activity. Thus, a combinational inhibition of
both TMMs will most likely be required for a successful global anti-cancer strategy. Since the current
lack of known ALT inhibitors is, according to leading researchers in the field, due to the absence of a
reliable and high-throughput assay for this type of cancer activity, we propose to develop high-
throughput versions of the common ALT activity assays to screen for potential genes in cancer cell lines
that are involved in the ALT pathway. Our results will potentially generate invaluable genetic targets for
the development of anti-cancer therapies that specifically shut down the ALT mechanism.

## Background

#### Introduction
It is estimated that somewhere between 10% to 15% of all cancer cells have no detectable
telomerase activity, and a significant proportion of these tumors rely on the alternative lengthening of
telomeres mechanism (ALT) (1,2) to maintain and/or elongate their telomeres through an as of yet poorly-
described mechanism(s) involving homologous recombination (3). The therapeutic importance of this field
is further highlighted by several studies reporting that some cancers contain both telomere
maintenance mechanisms (TMM), (4–9) and in vitro as well as preclinical data indicate that telomerase
inhibition may select for cancers that use ALT (10–13). Additionally, with the exception of gliomas, the
presence of TMM in tumors is often associated with poor prognosis and survival (7,8,14). In fact, detection
of ALT in liposarcomas and osteosarcomas is often associated with either the worst or just as poor
prognosis and survival for patients as telomerase is (8,15,16). Nonetheless, the majority of academic and
industry resources are currently directed toward telomerase as it is viewed as a nearly universal target
for cancer cells (3,17–19), but due to the perceived shortcomings of only targeting telomerase, cancer
researchers have proposed that the future of cancer therapies will involve combining inhibitors of both
TMM (1,12,20–22). This futuristic thinking is why the focus of the OncoSENS research team at Mountain View,
CA is on finding genes that are specific and essential to the ALT mechanism.

Given the minimal amount of support directed to researchers in the ALT field, it is no surprise
that it is far behind anti-telomerase therapy. For instance, as of July 2013, searching the term
‘telomerase’ on PubMed gives about 12,000 results while searching ‘alternative lengthening of
telomeres’ returns only 286 articles, which is merely about 2.4% of all telomerase-based work published
to date (Figure 1). Yearly publication trends for the telomerase and ALT fields (Figure 1) also suggest that
telomerase research dramatically expanded after the invention of the TRAP assay, but a similarly robust
assay capable of inducing a comparable trend for ALT has not been achieved yet. The gold standard for
ALT activity is telomere length maintenance in the absence of telomerase (3), but several ALT-associated
hallmarks have been identified. This type of TMM is thought to be dependent upon homologous
recombination and DNA damage repair proteins (23–25), and cells maintaining telomeres in this fashion are
reported to have heterogeneous telomere lengths, extra-chromosomal telomeric repeats (ECTR), which
include partially double-stranded C-rich circular DNA (C-circles), and ALT-associated promyelocytic
nuclear bodies (APBs) (26). It is hypothesized that ALT telomere synthesis is a recombination-based
mechanism that may be occurring in an APB (Figure 2) (23). Inhibition of several APB-associated
components or APB assembly in ALT-positive cells has been reported to induce senescence, cell death or
telomere shortening and are thus potential anti-cancer targets (3,27–30) (see also Supplementary Table 1).

Telomerase inhibitors are currently in clinical trials and it is widely believed that this is a result of
robust assays that allowed researchers and clinicians to reliably and quickly identify genes and
compounds that target this TMM (1,19). The telomerase field has been generating a wealth of data (Figure
1) for decades in the same format of the NCI 60 viability screen of the late 80s (31) with assays such as the
TRAP assay that originated in 1994 (32) and the subsequent miniaturizations (33), and high-content viability
assays that have developed since (19). Using current ALT assays, several genes have been identified that
modulate ALT activity, but virtually all these gene candidates are vital for many non-ALT cell functions
and thus are not ideal therapeutic candidates (3,10,25,27–29,34). Overall, the currently most reliable assays for ALT activity, namely C-circle (CC) and APB assays, are very low throughput as they require DNA dot
blotting (26), advanced qPCR techniques (35), or complex 3-dimensional confocal microscopy imaging (34), which
are all very labor and/or data intensive and thus not amenable to high-throughput screening of larger
gene databases. In sum, a TRAP assay equivalent for ALT activity has not materialized yet.

The OncoSENS team is working to overcome those limitations. We are using the same type of
low-throughput experiments described above to develop high-throughput assays for ALT activity. Our
team has had success transitioning the original CC Assay, which relies on radioactive probes, to a safer
luminescent reporter (DIG-based) format that does not require treatment of the samples with
restriction enzymes and thus yields results much faster. Additionally, we have had some preliminary
success in adapting the CC assay to a more high-throughput friendly, ELISA-based format (see below),
which eliminates the need for radioactive probes and DNA blotting altogether. As for the APB assay, the
advancements we have made in adapting this assay to work in a high-throughput fashion are even more
promising (see below). Our version of the APB assay replicates key published data without the need for
confocal microscopy or 3-D image reconstruction for quantitative analysis, which yields results faster
than the original assay (34).

In summary, we are developing the first truly high-throughput assays for ALT activity in cancer
cells. We hypothesize that by using these assays, we can quickly identify gene targets for ALT cancers by
screening large gene datasets by RNA interference. This would allow us to narrow down gene candidates
faster and focus on non-vital genetic targets that are unique to ALT activity and not required by every
cell in the body, which unfortunately is the drawback of virtually all of the ALT-associated genes
reported so far (Supplementary Table 1). The assays developed by this project could also be applied for
screening molecular compounds for drug development targeting ALT-positive cancers.

![ALT_publications_per_year](/assets/HT-ALT-Screen/ALT_publications_per_year.jpg)

Figure 1. Medline (PubMed) publication trends for telomerase and ALT research. The first telomerase
articles appeared in the late 80’s while ALT publications started in the mid to late 90’s. Arrows indicate
the invention of the most relevant assays for each field, namely the TRAP assay in 1994 (32), the APB assay
in 1999 (36) and the CC assay in 2009 (26). Source: Alexandru Dan Corlan. Medline trend: automated yearly statistics of PubMed results for any query, 2004. Web resource at URL:http://dan.corlan.net/medline-
trend.html. Accessed: 2013-07-23. (Archived by WebCite at http://www.webcitation.org/65RkD48SV)

![ALT_Telomere_Synthesis_Models](/assets/HT-ALT-Screen/ALT_Telomere_Synthesis_Models.jpg)

Figure 2. Proposed mechanisms of ALT activity. An RCA-based synthesis model involving circular
telomeric DNA may explain the presence of C-Circles (A), but the homologous recombination theory has
more support (B) 3 . The synthesis is believed to occur in an APB, which is composed of the assembly of
several different proteins (C) (23).

Unlike telomerase, which uses an RNA template and reverse transcriptase activity to modify
telomere length, ALT is believed to involve DNA repair and recombination enzymes and a linear or
circular DNA template (Figure 2) (1,3). This telomere synthesis activity is proposed to occur during the S
and G2 phases of the cell cycle inside APBs (Figure 2) (23,34,37). C-circles have been proposed to work as
DNA templates during elongation of telomeric repeats by rolling circle amplification (RCA), but it is
unclear so far if they are actively contributing to the ALT mechanism or are merely a by-product of
recombination-based telomere elongation by ALT (1,3,38). APBs were the first bona fide molecular markers of ALT activity identified in cancer cells (36). However, there are only two ALT-positive, in vitro SV40-immortalized cell lines, namely AG11395 and C3-c16, that do not possess APBs (26,39,40). Also, culture of ALT
cells in conditions that cause growth arrest and senescence were found to artificially increase the
formation of APBs (25,41).

## Current ALT Screening Methods

#### APB assay
The ALT-associated promyelocytic body (APB) assay was the first alternative lengthening of
telomeres (ALT) assay to be developed. Prior to its discovery in 1999 36 (see Figure 1), the only known
criteria for determining the presence of ALT activity were long and heterogeneous telomere
maintenance and undetectable telomerase activity by the TRAP assay 36 . This assay involves testing for
colocalization of telomeric DNA and promyelocytic body protein (PML). Though PML plays a role in a
variety of functions from senescence to proliferation (42), it is very rarely found at the telomeres (34). Mortal
and telomerase-positive (TEL+) cells typically have at most two or less APBs per nuclei, while established
ALT-positive (ALT+) cell lines and those in the process of immortalization by ALT are reported to have in
excess of four (34,36).

This has led to the use of the APB assay in the search for genes involved in ALT (25,27,34) as well as
for determining telomere maintenance mechanisms in patient tumor samples (7,43). Detection of APBs in
tumors has been reported to have prognostic significance in various types of cancer (7,43). For years,
different image acquisition setups, counting methods, and culture conditions have led to various
numbers of APBs to be reported by different groups (25,36,44–46). Recently, an improved method for
detecting and counting APBs was reported 34 in which confocal imaging and 3-D image reconstruction
combined with colocalization techniques were used to determine the impact of various siRNAs on the
number of APBs per cell (34). Though this new 3-D assay has been exciting for the field, image acquisition
alone requires about 17-34 hours per slide (384 spots) while image analysis using a multi-node
supercomputer takes about 6-8 hours (23-42 hours total) and it is thus very impractical for high-
throughput screening. Nonetheless, this 3-D APB assay is one of the most detailed screening analyses to
date, and the key data are summarized in Figure 3 (34). U2OS cells (Figure 3A) have on average 4.4 APBs
per nuclei with the distribution shown in Figure 3B, with over 90% of U2OS cells having 1 or more APBs,
while HeLa cells have only 0.5 APBs per nuclei on average (Figure 3C) with only about 34% of these cells
containing colocalizations. Analysis of the size of both telomeres and PML in APBs shows that these are
enlarged inside APBs as compared to the ones outside of these bodies (Figure 3D-E). Since the APB assay
in its current format has limited investigators to screening a maximum of 9-14 genes in a single
study (25,34), we have developed an improved APB assay format optimized for high-throughput screening,
which is fully described in more detail below.

![APB_assay](/assets/HT-ALT-Screen/APB_assay.jpg)

Figure 3. Current methods of detecting and counting APBs in cancer cell lines. Immunofluorescence
images of APBs as reported in the literature for ALT+ U2OS cells (A). Note that yellow indicates
colocalization of PML and TRF2 in nuclei here. Published methods for automated counting of APBs have
yielded statistically significant results in ALT+ U2OS (B) and TEL+ HeLa (C). The size of telomeres (D) and
PML (E) in APBs is larger than in foci outside of APBs.

#### C-circle Assay
Extra-chromosomal telomeric repeats (ECTR) are one of the major phenotypes reported in ALT+
cells . The various ECTR types include: G-circles, C-circles (CC), and t-circles (3). Though there are
various differences in the abundance of these circles among mortal, ALT and telomerase cell lines, the
presence of CC at high levels is the most tightly correlated phenotype with ALT activity identified so
far (26). The presence of CC in 38 cancer cell lines isolated from various tissues and immortalized through a
myriad of different ways is a testament to the strength of the CC assay (26). CC appear during
immortalization at the same time as other markers of ALT activity (e.g., APBs) and they gradually
decrease to undetectable levels the more ALT activity is inhibited (26).

This assay has been successfully used to identify ALT as the telomere maintenance mechanism
from blood samples of osteosarcoma patients and to confirm that many of the genes previously known
to be involved in ALT also affect CC levels (26). Though its isothermal expansion steps make this assay
suitable to use by more labs without a PCR machine, the applicability of the original assay to high-
throughput screening is very limited (26). It requires 3-4 days of very extensive amplification, blotting,
labeling and developing steps as well as a radioactive probe (26) (Figure 4A), which is not an option for many research and diagnostic labs. A quantitative PCR-based version that can be done slightly faster does exist (35), but it is even more labor intensive in both the setup and data analysis, and thus it is not
very high-throughput friendly. We have developed a non-radioactive version of the original C-circle
assay that takes less time to complete (Figure 6A-B), but it still requires DNA blotting and as such is not
suitable for a high-throughput screening format. We are developing a high-throughput, ELISA-based
version of the CC assay and it will be further described in the next section (see Figure 6).

![C-circle-assay](/assets/HT-ALT-Screen/C-circle-assay.jpg)

Figure 4. The C-circle assay is tightly correlated with ALT activity (26). To test for the presence of C-Circles,
circular DNA present in samples is used as a template by phi29 DNA polymerase to produce linear
sequences which are then probed for the resultant G-rich, telomeric repeat strands (A). This radioactive
assay has been reported to accurately measure ALT activity in 38 different cell lines (B). Typical CC assay
results for a panel of ALT+ and TEL+ cell lines, as well as artificial CC (C96) samples is shown (C).

## Preliminary Data

#### 2-D APB assay
It has been previously reported that automated APB screenings can take up to 34 hours per
slide, but it can hypothetically be set up to only take 17 hours 34 . The total time to screen 3 slides of 384
spots each is about 72 hours (24 hours per slide) in the best case scenario (600-1200 cells total per
condition, 11 genes or conditions total). With this limitation in mind we set out to look for ways of
making this assay more high-throughput friendly and less data intensive. Using the Molecular Devices
IXM high-throughput screening microscope (Supplementary Figure 1) and customized software
algorithms for data collection and analysis, we achieved very exciting results (Figure 5).

We are currently
able to acquire, detect and quantify the APBs in cells seeded on a full 96-well plate in just about 2.5-3.5
hours (Figure 5), with 150-300 cells analyzed per condition. We can thus complete an APB screen of
four full 96-well plates (384 wells total) in about 14 hours (600-1200 total cells per condition, 12 genes
or conditions total), which is more than 5 times faster than the hypothetical maximum speed per
screen reported in the literature 34 . And this can be accomplished without using a supercomputer for
image analysis since we only need to analyze less than 48,000 images per screen in 2-D versus the
780,000 images in 3-D in the current automated method 34 . Our assay also does not rely on artificially increasing APB formation by creating senescence culture conditions (25). Our data reproduces key APB
parameters reported in the literature, (34) including distribution of APBs per nuclei in ALT+ and TEL+ cells
(Figure 5B-C), the average number of APBs per nuclei in these cells (Figure 5D), the percent of cells
containing at least 1 APB per nuclei (Figure 5E), and the shift in the size of telomeres and PML (Figure
5F-G). Our assay also revealed new data on the lack of an effect of POT1 gene knockdown on APB
formation in 143B (TEL+) cells (Figure 5D).

![imaging-technique-2d](/assets/HT-ALT-Screen/2d-apb-assay.jpg)

Figure 5. The two-dimensional APB assay is capable of screening multiple samples at once at high
speeds.(A) Representative fluorescent images of GM00847, U2OS, 143B, and 143B cells transfected with
a POT1 knockdown construct from our high-throughput 2-D APB assay taken with Molecular Devices
IXM using customized deconvolution and z-stack projection scripts. Our immunofluorescence-based 2-D
APB high-throughput detection method yields colocalization numbers similar to those reported in the
literature (B-E) (34). Telomeres (F) and PML (G) increase in size, as measured by area (μm 2 ), when present
in APBs. See also Figure 3 for comparison with the 3-D APB automated detection method.

#### ELISA-based CC assay
As described previously, the challenges associated with the CC assay limit its use to mainly low-
throughput experiments (26,35). We are attempting to overcome that hurdle by incorporating detection
technologies into the assay that are more amenable to high-throughput screening. We already succeeded in creating a non-radioactive version of the assay (Figure 6A-B), which reproduces the main
results from the original CC assay study 26 (Figure 4C). We are now working to make the CC assay
detectable by ELISA using biotin-labeled capture probes and DIG-labeling the phi29-expanded RCA
products (Figure 6C-D), which shorten time to detection and greatly simplify data collection and
quantification. The goal is to achieve a high-throughput assay for CC like the TRAP assay is for
telomerase activity (19).

We had reasonably preliminary success with detecting CC amplification signals
from ALT+ cell lines as quickly as less than 24 hours (Figure 6C-D), but significant work still needs to be
done to improve the sensitivity and reproducibility of the assay. Once this assay is further developed, it
could be used in addition to the 2-D APB assay described above to perform high-throughput genetic
screens on ALT-associated genes. Also, the ELISA-based CC assay could potentially yield results in as
little as 16-18 hours from sample DNA isolation to detection as opposed to the 2-4 days currently
required for the original CC assay.

![ELISA-CC_assay](/assets/HT-ALT-Screen/ELISA-CC_assay.jpg)

Figure 6. Development of novel C-circle assays by the OncoSENS team. The non-radioactive version of
the CC assay shows similar sensitivity to the original assay (26) (A-B).The ELISA-based CC assay attempts to
incorporate the successful high-content aspects of the TRAP assay for telomerase activity into a C-circle
assay format as shown in (C-D). Though we are still exploring several different sample preparation methods to increase sensitivity and reproducibility, we can report successful detection of positive
controls (C) and ALT+ samples for the assay (D). Heating as well as chemically mediated cleavage (D) of
the RCA telomeric strands derived from CC show promising results. The intensity of the green color is
directly proportional to the amount of sample detected by the assay.

## Research Plan
#### Rationale and Expected Impact
* The ALT cancer field currently lacks robust assays and funding as compared to telomerase-
based cancer research.
* Our goal is to develop and establish functional high-throughput and high-content ALT assays
that are useful for testing patient samples, quickly identifying gene targets, screening for small
molecule drugs, and accelerating research on ALT mechanisms in general.
* Our group will use these screening methods to identify genes that are essential for ALT activity
in cancer cell lines.
* These ALT genes will provide the cancer research field with a wealth of therapeutic candidates
and leads in the investigation of how the ALT mechanism works.
* The assays developed in this project ma also grow the scientific interest in the ALT field.

#### Strategy and Methodology
We will fully establish our two-dimensional (2-D) APB assay and work on optimizing the ELISA-
based, high-throughput version of the CC assay.
* The most comprehensive siRNA 3-D APB screen performed to date will be replicated with our
two-dimensional assay and the CC ELISA assay once it is functional.
* Our assays will also be used to screen other genes that have been reported to modulate ALT
activity by assays other than APB (see Supplementary Table 1).
* Cell lines representative of a variety of cancer types and telomere maintenance mechanisms will
be screened with these high-throughput assays to quickly identify genes involved in ALT (Figure
7).
* These cell lines will then be tested for genes that have been validated as modulators of ALT
activity (Supplementary Table 1) as well as several other genes that are reportedly differentially
expressed in ALT+ versus TEL+ cells 48 but that have not been functionally tested by any ALT-
related assay yet (Figure 8).
* In the long-term, stable cell lines expressing genes of interest or shRNAs to target genes will be
created and tested using our in vitro high-throughput ALT assays as well as others: C-Circle
assay, APB assay, telomere length determination by qPCR and cell viability (Figure 8).
* In vivo studies on the stable cell lines will be performed to establish a correlation between lack
of ALT activity and the tumorigenicity of these cells as well as survival of experimental animals
(Figure 8).
* Information will be shared with the field through national and international conferences and
publications.

![siRNA_screen](/assets/HT-ALT-Screen/siRNA_screen.jpg)

Figure 7. Strategy for siRNA screen using a library created from published ALT-associated gene targets.
Cancer cell lines will be subjected to siRNA screen for several genes with at least 2 plates for each screen
such that one plate will be assayed for APBs and the other for cell viability. Each plate will have columns
1 and 2 reserved for controls, as outlined above. See also Supplementary Table 1 for the genes of
interest for validating the high-throughput assays for ALT activity.

![screen-workflow](/assets/HT-ALT-Screen/screen-workflow.jpg)

Figure 8. Workflow diagram of the long-term OncoSENS strategy for high-content screening and
validation of ALT-associated genes. Microarray gene expression datasets from TEL+ vs ALT+ cells will
serve as gene target inputs for our siRNA screen using both types of cancer cells. Genes overexpressed
in ALT+ cells but downregulated in TEL+ cells will be knocked down in ALT cells via siRNAs and analyzed
using high-content assays. Similarly, genes overexpressed in TEL+ but not in ALT+ cells will be
downregulated in TEL+ cells via siRNA. The gene targets identified this way will be used to generate
stable cell lines for further in vitro and in vivo testing to confirm ALT-associated activity and their
potential as a therapeutic candidate.

#### Specific Aims
1. Validate high-throughput ALT activity assays via RNA interference screens on ALT+ cells
targeting genes that have already been found in the literature to modulate ALT activity.
2. Using our high-content ALT assays, perform siRNA screen on ALT+ cells for the genes
overexpressed in ALT+ but not TEL+ cells.
3. Using our high-content ALT assays, perform siRNA screen on TEL+ cells for the genes
overexpressed in TEL+ but not ALT+ cells.

## Research Methods

#### Cell lines, Transfection, siRNA library
A panel of three ALT+ cell lines and three TEL+ cell lines will be obtained from ATCC. The REQUIRES
FINAL UPDATED FORMAT siRNA library detailed in Supplementary Table 1 will be obtained from TBD
ORGANIZATION in 96-well plate format. The gene silencing and cell viability determination methods
from a recent high-throughput screen of telomerase inhibitors 19 will be used. Stable cell lines will be
generated from genes of interest identified by high throughput screening will be performed as
previously described (19).
#### ELISA-based CC Assay Development
Cells will be treated as per an established C-Circle expansion protocol and various detection, probing,
cleaving and expansion techniques will be tested. Incorporation testing will include ddATP, biotin dATP,
DIG dUTP, dUTP. Sample treatment may involve heating, telomeric PCR primer expansion, vortexing,
uracil DNA glycosylase treatment, duplex specific nuclease, sonication, denaturation. Detection
methods screened will include PCR and ELISA.
#### 2-D APB Assay
Colocalized TRF2 and PML will be labeled as described previously 36 and detected in a high throughput
fashion by collapsing 3-D stacks into 2-D images and performing image analysis with a Molecular Devices
script.
#### CTG Viability Assay
Cell viability will be assessed with the CTG viability assay as per manufacturer protocol.
#### Telomere Length Determination
Telomere length will be determined with an established qPCR-based detection method (49).
#### CC Assay
The C-Circle assay will be performed as previously described by the Reddel group 26 with alterations of
luminescent detection and DNA shearing methods that we have developed at SENS.


# References
1. Shay, J. W., Reddel, R. R. & Wright, W. E. Cancer and Telomeres—An ALTernative to Telomerase.
Science 336, 1388–1390 (2012).
2. Heaphy, C. M. et al. Prevalence of the alternative lengthening of telomeres telomere maintenance
mechanism in human cancer subtypes. Am. J. Pathol. 179, 1608–1615 (2011).
3. Cesare, A. J. & Reddel, R. R. Alternative lengthening of telomeres: models, mechanisms and
implications. Nat. Rev. Genet. 11, 319–330 (2010).
4. Gocha, A. R. S., Nuovo, G., Iwenofu, O. H. & Groden, J. Human sarcomas are mosaic for telomerase-
dependent and telomerase-independent telomere maintenance mechanisms: implications for
telomere-based therapies. Am. J. Pathol. 182, 41–48 (2013).
5. Costa, A. et al. Telomere maintenance mechanisms in liposarcomas: association with histologic
subtypes and disease progression. Cancer Res. 66, 8918–8924 (2006).
6. Henson, J. D. et al. A Robust Assay for Alternative Lengthening of Telomeres in Tumors Shows the
Significance of Alternative Lengthening of Telomeres in Sarcomas and Astrocytomas. Clin Cancer Res
11, 217–225 (2005).
7. Hung, N. A. Telomere Maintenance Mechanisms: Prognostic and Therapeutic Implications for the
Pathologist and Oncologist. Open Journal of Pathology 03, 10–20 (2013).
8. Ulaner, G. A. et al. Absence of a Telomere Maintenance Mechanism as a Favorable Prognostic Factor
in Patients with Osteosarcoma. Cancer Res 63, 1759–1763 (2003).
9. Venturini, L. et al. Telomere maintenance mechanisms in malignant peripheral nerve sheath tumors:
expression and prognostic relevance. Neuro-oncology 14, 736–744 (2012).
10. Hu, J. et al. Antitelomerase therapy provokes ALT and mitochondrial adaptive mechanisms in
cancer. Cell 148, 651–663 (2012).
11. Xue, Y. et al. Twisted Epithelial-to-Mesenchymal Transition Promotes Progression of Surviving
Bladder Cancer T24 Cells with hTERT-Dysfunction. PLoS ONE 6, e27748 (2011).
12. Chen, W. et al. Telomerase inhibition alters telomere maintenance mechanisms in laryngeal
squamous carcinoma cells. J Laryngol Otol 124, 778–783 (2010).
13. Chen, W., Xiao, B.-K., Liu, J.-P., Chen, S.-M. & Tao, Z.-Z. Alternative lengthening of telomeres in
hTERT-inhibited laryngeal cancer cells. Cancer Sci. 101, 1769–1776 (2010).
14. Hakin-Smith, V. et al. Alternative lengthening of telomeres and survival in patients with
glioblastoma multiforme. The Lancet 361, 836–838 (2003).
15. Cairney, C. J., Hoare, S. F., Daidone, M.-G., Zaffaroni, N. & Keith, W. N. High level of telomerase
RNA gene expression is associated with chromatin modification, the ALT phenotype and poor
prognosis in liposarcoma. Br. J. Cancer 98, 1467–1474 (2008).
16. Venturini, L., Motta, R., Gronchi, A., Daidone, M. & Zaffaroni, N. Prognostic relevance of ALT-
associated markers in liposarcoma: a comparative analysis. BMC Cancer 10, 254 (2010).
17. Shay, J. W., Zou, Y., Hiyama, E. & Wright, W. E. Telomerase and cancer. Hum. Mol. Genet. 10,
677–685 (2001).
18. Harley, C. B. Telomerase and cancer therapeutics. Nat. Rev. Cancer 8, 167–179 (2008).
19. Cerone, M. A., Burgess, D. J., Naceur-Lombardelli, C., Lord, C. J. & Ashworth, A. High-throughput
RNAi screening reveals novel regulators of telomerase. Cancer Res. 71, 3328–3340 (2011).
20. Folini, M., Gandellini, P. & Zaffaroni, N. Targeting the telosome: therapeutic implications.
Biochim. Biophys. Acta 1792, 309–316 (2009).
21. Wang, Q. et al. G-quadruplex formation at the 3? end of telomere DNA inhibits its extension by
telomerase, polymerase and unwinding by helicase. Nucleic Acids Res 39, 6229–6237 (2011).
22. Temime-Smaali, N. et al. The G-Quadruplex Ligand Telomestatin Impairs Binding of
Topoisomerase IIIα to G-Quadruplex-Forming Oligonucleotides and Uncaps Telomeres in ALT Cells.
PLoS ONE 4, e6919 (2009).
23. Chung, I., Osterwald, S., Deeg, K. I. & Rippe, K. PML body meets telomere: the beginning of an
ALTernate ending? Nucleus 3, 263–275 (2012).
24. Chung, I., Leonhardt, H. & Rippe, K. De novo assembly of a PML nuclear subcompartment occurs
through multiple pathways and induces telomere elongation. J. Cell. Sci. 124, 3603–3618 (2011).
25. Jiang, W.-Q., Zhong, Z.-H., Henson, J. D. & Reddel, R. R. Identification of candidate alternative
lengthening of telomeres genes by methionine restriction and RNA interference. Oncogene 26, 4635–
4647 (2007).
26. Henson, J. D. et al. DNA C-circles are specific and quantifiable markers of alternative-
lengthening-of-telomeres activity. Nat. Biotechnol. 27, 1181–1185 (2009).
27. Jiang, W.-Q. et al. Suppression of alternative lengthening of telomeres by Sp100-mediated
sequestration of the MRE11/RAD50/NBS1 complex. Mol. Cell. Biol. 25, 2708–2721 (2005).
28. Wu, G., Jiang, X., Lee, W.-H. & Chen, P.-L. Assembly of functional ALT-associated promyelocytic
leukemia bodies requires Nijmegen Breakage Syndrome 1. Cancer Res. 63, 2589–2595 (2003).
29. Bhattacharyya, S. et al. Telomerase-associated Protein 1, HSP90, and Topoisomerase IIα
Associate Directly with the BLM Helicase in Immortalized Cells Using ALT and Modulate Its Helicase
Activity Using Telomeric DNA Substrates. J. Biol. Chem. 284, 14966–14977 (2009).
30. Stagno D’Alcontres, M., Mendez-Bermudez, A., Foxon, J. L., Royle, N. J. & Salomoni, P. Lack of
TRF2 in ALT cells causes PML-dependent p53 activation and loss of telomeric DNA. J. Cell Biol. 179,
855–867 (2007).
31. Shoemaker, R. H. The NCI60 human tumour cell line anticancer drug screen. Nat. Rev. Cancer 6,
813–823 (2006).
32. Kim, N. W. et al. Specific association of human telomerase activity with immortal cells and
cancer. Science 266, 2011–2015 (1994).
33. Heller-Uszynska, K. & Kilian, A. Microarray TRAP--a high-throughput assay to quantitate
telomerase activity. Biochem. Biophys. Res. Commun. 323, 465–472 (2004).
34. Osterwald, S. et al. A three-dimensional colocalization RNA interference screening platform to
elucidate the alternative lengthening of telomeres pathway. Biotechnol J 7, 103–116 (2011).
35. Lau, L. M. S. et al. Detection of alternative lengthening of telomeres by telomere quantitative
PCR. Nucleic Acids Res. 41, e34 (2013).
36. Yeager, T. R. et al. Telomerase-negative immortalized human cells contain a novel type of
promyelocytic leukemia (PML) body. Cancer Res. 59, 4175–4179 (1999).
37. Wu, G., Lee, W. H. & Chen, P. L. NBS1 and TRF1 colocalize at promyelocytic leukemia bodies
during late S/G2 phases in immortalized telomerase-negative cells. Implication of NBS1 in alternative
lengthening of telomeres. J. Biol. Chem. 275, 30618–30622 (2000).
38. Oganesian, L. & Karlseder, J. Mammalian 5’ C-rich telomeric overhangs are a mark of
recombination-dependent telomere maintenance. Mol. Cell 42, 224–236 (2011).
39. Fasching, C. L., Bower, K. & Reddel, R. R. Telomerase-independent telomere length maintenance
in the absence of alternative lengthening of telomeres-associated promyelocytic leukemia bodies.
Cancer Res. 65, 2722–2729 (2005).
40. Cerone, M. A., Autexier, C., Londoño-Vallejo, J. A. & Bacchetti, S. A human cell line that
maintains telomeres in the absence of telomerase and of key markers of ALT. Oncogene 24, 7893–
7901 (2005).
41. Jiang, W.-Q. et al. Induction of alternative lengthening of telomeres-associated PML bodies by
p53/p21 requires HP1 proteins. J Cell Biol 185, 797–810 (2009).
42. Lallemand-Breitenbach, V. & de The, H. PML Nuclear Bodies. Cold Spring Harb Perspect Biol 2,
(2010).
43. Venturini, L. et al. ALT-associated promyelocytic leukaemia body (APB) detection as a
reproducible tool to assess alternative lengthening of telomere stability in liposarcomas. J. Pathol.
214, 410–414 (2008).
44. Perrem, K., Colgin, L. M., Neumann, A. A., Yeager, T. R. & Reddel, R. R. Coexistence of alternative
lengthening of telomeres and telomerase in hTERT-transfected GM847 cells. Mol. Cell. Biol. 21, 3862–
3875 (2001).
45. Fasching, C. L., Neumann, A. A., Muntoni, A., Yeager, T. R. & Reddel, R. R. DNA damage induces
alternative lengthening of telomeres (ALT) associated promyelocytic leukemia bodies that
preferentially associate with linear telomeric DNA. Cancer Res. 67, 7072–7077 (2007).
46. Nabetani, A., Yokoyama, O. & Ishikawa, F. Localization of hRad9, hHus1, hRad1, and hRad17 and
caffeine-sensitive DNA replication at the alternative lengthening of telomeres-associated
promyelocytic leukemia body. J. Biol. Chem. 279, 25849–25857 (2004).
47. Cesare, A. J. & Griffith, J. D. Telomeric DNA in ALT cells is characterized by free telomeric circles
and heterogeneous t-loops. Mol. Cell. Biol. 24, 9948–9957 (2004).
48. Lafferty-Whyte, K. et al. A gene expression signature classifying telomerase and ALT
immortalization reveals an hTERT regulatory network and suggests a mesenchymal stem cell origin
for ALT. Oncogene 28, 3765–3774 (2009).
49. Cawthon, R. M. Telomere measurement by quantitative PCR. Nucl. Acids Res. 30, e47–e47
(2002).

# Appendix A: Supplementary Information

![imaging-technique-2d](/assets/HT-ALT-Screen/imaging-technique-2d.jpg)

Supplementary Figure 1. Comparison of image acquisition techniques used by the current 3-D APB
colocalization assay 34 (A) and the two-dimensional 2-D APB assay that we have developed in
collaboration with Molecular Devices (B).

# Supplementary Table 1

![ALT-genes](/assets/HT-ALT-Screen/ALT-genes.jpg)

Genes of interest for initial validation of high-throughput screenings. All the
genes below have been found in previous publications to have some impact on ALT cells or ALT activity
by different assays such as APB, CC, T-SCE, t-circles or ECTRs, TRFL, C-rich overhangs, and proliferation.
These genes will be used in the first screen to validate the high-throughput version of the APB assay
before we perform any further screening of gene candidates.
