---
layout: post
title:  "Validating the Mesenchymal ALT Gene Signature"
date:   2019-01-06 22:42:40 -0700
categories: Biology Stem_Cells ALT Sequencing
---
Lafferty-Whyte 2009 A gene expression signature classifying telomerase and ALT immortalisation reveals an hTERT regulatory network and suggests a mesenchymal stem cell origin for ALT
==================

gene expression signature distingusih ALT vs TEL published by lafeerty white. from interesction two independent signatures from cell lines and liposarcoma tumors WHICH UTILIZE differents TMMs.
this current suty used U133plus2.0 arrays
(Affymetrix, Santa Clara, CA, USA) to do similar analysis of indepdent liposarcomas with defined TMMs.
FOR OUR DATASETS using the 297 gene signature causes liposarcoms to cluster on TUMOR HISTOLOGICAL SUBTYPE, NOT TMM!!!

Histological type (WD, well differentiated; MYX, myxoid; RC, round cell; DD, dedifferentiated; PLEO,
pleomorphic; LS NOS, liposarcoma not otherwise specified) and TMM are indicated, with ‘NA’ used for tumors that were not clearly
ALT or telomerase-positive.
(a) Heatmap of 38 tumors representing all histological subtypes of liposarcoma. (b) Heatmap of only
dedifferentiated liposarcoma samples.
figure 1
contrlling for histoloigcla subtypes, restricted to didifferentiated liposarcomas. linear modeling for microsarrays NO GENES significantly changed. pre filedtered data led to 14 gene signature WITH NO GNES IN COMMON WITH 297 GENE SINGATURE
also did unsupervised clustering of dedifferentiated tumor data and FOUND NO STRONG CORRELATION BETWEEN GENE EXPRESSION AND TMM.
maybe micorarray platoform diffeernce and tumor smaples used??? prob NOT
ORIGINAL CELL LINES used differed not only in TMM, but also tissue of origin, with 75% teloemrase positive cell lines of epithelial origin and 75% of ALT lines being of firbroblastic origin.
initial gene signature could jus be strong singauter of cell type and NOT TMM.
see table 1 of cairney 2008: ALT tumors mostly dedifferentiated liposarcomas, and telomerase tumors are mostly myxoidround cell liposarcoams.
ALT vs TEL from this data set is messed by histological subtypes.
the 297 gene signature is mostly dedifferentiation state (FIGURE 1A.)
ALT tumors biased for dedifferntiated liposarcomas. expresison signature of dedifferentiated liposarcoma more closely resembles mesenchymal stem cells than myoxid/round cell liposarcoma. this pcould dexplain why ALT tumors appear to cluster w/ mesenchym stem clel samples. OUR observation couldn't replicate. WE think it's differentiation differences for m histoligcal subtypes .

![Doyle_2012](/assets/Validating_Signature/Doyle_2012.png)
Doyle 2012 Validating a gene expression signature proposed to differentiate liposarcomas that use different telomere maintenance mechanisms


====================

CLARIFICATION: we only aimed to get molecular mechanism sna dnetworks of TMM in liposarcoma. 
also showed network analysis and functional validation with qPCR and wester blotting in a range of cell lines.
we think othe letter has interesting points, but that it's preliminary and unsubstantiated.
different microarray platforms as Affymetrix and Aglinet are different.
we see the authors mention that some genes are absetn.
other authors preselcted single probe with higest median expression. IN OCNTRAST we identified probles divergent expression betwen TMM. their gene list won't be idnetical to ours.
 ALSO other authors don't mention specific probles in thier GEO submission.
 ALSO sample handlign information mising from that submisison. is it biological or technical variance?
 PRINCIPAL COMPONENT ANALYSIS of ALT and TMM from new data set suggets that tehcnical variation from date of the arrays getting scanned is the largest factor for smaple grouping (outweight biological differences including histolgical subtype and TMM).
 we also identify other issues that make other authors iddferent than us.
 ALSO pca IN FIGURE 1 SUGGETS THAT OTHER AUTHORS OWN SAMPLES ARE INTERNALLY INCOMPARABLE.
 the others of other letter use both trf and apb DESPITE ONLY 80% AGREEMENT WITH THOSE APPROACHES. we only use apb detection.
 SOME SAMPLES WERE ASSIGNED UNKOWN tmm WITOUT TESTING apb.
 OUR DATA ALSO HAD msc WHICH AWERE ABSENT FORM ATUHROS. THE AUTHORS INSTQEAD HAVE LIPOSARCOMA SAMPLES THAT ARE NEITHER alt NOR TELOMERASE.

OUR STUDY DESING WASNTED TO DISTINGUE alt FROM tel, BUT ALSO LEARN UNKNWON REGULATORY MECHANISM OF tmm.

![Keith_2012](/assets/Validating_Signature/Keith_2012.png)



Keith 2012 Response to ‘Validating a gene expression signature proposed to differentiate liposarcomas that use different telomere maintenance mechanisms’
