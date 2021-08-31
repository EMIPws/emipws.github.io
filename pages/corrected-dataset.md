---
layout: single
permalink: /corrected-dataset/
header:
title: "Distributed Collection of Eye Movement Data in Programming - Corrected Dataset"
sidebar:
  nav: "main"
---

In an effort to make the EMIP dataset more accessible and easier to use, Al Madi et al. presented a corrected token-level version of the EMIP dataset.

**Download:**

The corrected dataset can be [downloaded from the following link](https://osf.io/djn9s/)

# EMIP Toolkit

In addition to the corrected dataset, the paper presents EMIP Toolkit (EMTK), which is a **Python** library for customized post-processing of the EMIP dataset. EMTK implements the following features:
 
* Parsing raw data files from the EMIP dataset into Experiment, Trial, and Fixation containers.
* Customizable dispersion-based fixation detection algorithm implementation according to the manual of the SMI eye tracker used in the data collection.
* Raw data and filtered data visualizations for each trial.
* Performing hit testing between fixations and AOIs to determine the fixations over
each AOI.
* Customizable offset-based fixation correction implementation for each trial.
* Customizable Areas Of Interest (AOIs) mapping implementation at the line level
or token level in source code for each trial.
* Visualizing AOIs before and after fixations overlay on the code stimulus.
* Mapping source code tokens to generated AOIs and eye movement data.
* Adding source code lexical category tags to eye movement data using [srcML](https://www.srcml.org/). srcML is a static analysis tool and data format that provides very accurate syntactic categories (method signatures, parameters, function names, method calls, declarations and so on) for source code.

# EMIP Toolkit Download:

A stable version of the EMTK can be [downloaded through the replication package here](https://osf.io/djn9s/).

The replication package contains a Jupyter Notebook file "EMIP_Toolkit_Examples.ipynb" that contains examples and a tutorial on using the EMIP Toolkit. The latest development version of the [EMTK can be found here](https://github.com/nalmadi/EMIP-Toolkit).
  
# Paper:

The details of the correction process and Toolkit features are presented [in this paper](https://www.researchgate.net/publication/350485560_EMIP_Toolkit_A_Python_Library_for_Customized_Post-processing_of_the_Eye_Movements_in_Programming_Dataset).

**Video presentation:**
<iframe width="560" height="315" src="https://www.youtube.com/embed/wFdGyM6qUlE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**Please cite this paper:**

Naser Al Madi, Drew T. Guarnera, Bonita Sharif, and Jonathan I. Maletic.2021. EMIP Toolkit: A Python Library for Customized Post-processing of the Eye Movements in Programming Dataset. In ETRA ’21: 2021 Symposium on Eye Tracking Research and Applications (ETRA ’21 Short Papers), May25–27, 2021, Virtual Event, Germany. ACM, New York, NY, USA, 6 pages. [https://doi.org/10.1145/3448018.3457425](https://doi.org/10.1145/3448018.3457425)
