---
layout: post
title:  "Hight-Throughput-APB-Assay"
date:   2018-12-18 22:42:40 -0700
categories: Biology
---

# High-Throughput APB Assay

It has been previously reported that automated APB screenings can take up to 34 hours per slide, but it can hypothetically be set up to only take 17 hours (Osterwald 2011). The total time to screen 3 slides of 384 spots each is about 72 hours (24 hours per slide) in the best case scenario (600-1200 cells total per condition, 11 genes or conditions total). With this limitation in mind we set out to look for ways of making this assay more high-throughput friendly and less data intensive. Using the Molecular Devices IXM high-throughput screening microscope (Supplementary Figure 1) and customized software algorithms for data collection and analysis, we achieved very exciting results (Figure 5). We are currently able to acquire, detect and quantify the APBs in cells seeded on a full 96-well plate in just about 2.5-3.5 hours (Figure 5), with 150-300 cells analyzed per condition. We  can thus complete an APB screen of four full 96-well plates (384 wells total) in about 14 hours (600-1200 total cells per condition, 12 genes or conditions total), which is more than 5 times faster than the hypothetical maximum speed per screen reported in the literature (Osterwald 2011). And this can be accomplished without using a supercomputer for image analysis since we only need to analyze less than 48,000 images per screen in 2-D versus the 780,000 images in 3-D in the current automated method (Osterwald 2011). Our assay also does not rely on artificially increasing APB formation by creating senescence culture conditions (Jiang 2007). Our data reproduces key APB parameters reported in the literature,(Osterwald 2011) including distribution of APBs per nuclei in ALT+ and TEL+ cells (Figure 5B-C), the average number of APBs per nuclei in these cells (Figure 5D), the percent of cells containing at least 1 APB per nuclei (Figure 5E), and the shift in the size of telomeres and PML (Figure 5F-G). Our assay also revealed new data on the lack of an effect of POT1 gene knockdown on APB formation in 143B (TEL+) cells (Figure 5D).

![2d-apb-assay]/Assets/ALT_Synthesis_Models/2d-apb-assay.jpg ("2d-apb-assay")


Figure 5. The two-dimensional APB assay is capable of screening multiple samples at once at high speeds.(A) Representative fluorescent images of GM00847, U2OS, 143B, and 143B cells transfected with a POT1 knockdown construct from our high-throughput 2-D APB assay taken with Molecular Devices IXM using customized deconvolution and z-stack projection scripts. Our immunofluorescence-based 2-D APB high-throughput detection method yields colocalization numbers similar to those reported in the literature (B-E)34. Telomeres (F) and PML (G) increase in size, as measured by area (µm2), when present in APBs. See also Figure 3 for comparison with the 3-D APB automated detection method.

# Citations
Osterwald, S. et al. A three-dimensional colocalization RNA interference screening platform to elucidate the alternative lengthening of telomeres pathway. Biotechnol J 7, 103–116 (2011).
Jiang, W.-Q., Zhong, Z.-H., Henson, J. D. & Reddel, R. R. Identification of candidate alternative lengthening of telomeres genes by methionine restriction and RNA interference. Oncogene 26, 4635–4647 (2007).
