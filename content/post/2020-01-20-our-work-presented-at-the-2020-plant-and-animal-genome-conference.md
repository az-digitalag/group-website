---
title: Our work presented at the 2020 Plant and Animal Genome Conference
authors: 
- David LeBauer
date: '2020-01-20'
slug: our-work-presented-at-the-2020-plant-and-animal-genome-conference
categories: []
tags: []
subtitle: ''
summary: ''
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---

![PAG](/post/2020-01-20-our-work-presented-at-the-2020-plant-and-animal-genome-conference_files/2020-PAG-xxviii-d6ee726f.jpg)

The Plant and Animal Genome XXVIII conference (PAG) is the largest agricultural genomics conference in the world, and there is a lot of interest in statistics, sensing, data sharing, and software. PAG is held each year in San Diego, and this year's conference was a great opportunity for me (David) to share the work from our group and learn about a wide range of research, software, and data in the domains of agriculture, high throughput phenomics, and genomics.

There were many great talks and informal conversations with current and (hopefully!) future collaborators. A few of the presentations that described work in our group included:

1. My presentation at the workshop “Challenges and Opportunities in Plant Science Data Management”. Darwin Campbell, Carolyn Lawrence-Dill, Ian Brown, and Robert Davey organized the workshop. My talk was titled “Software to Streamline Sharing of Agricultural Algorithms and Data” ([abstract](https://plan.core-apps.com/pag_2020/abstract/926b92fd-a248-49e8-b7fb-5c4961dd7eda)). It described our efforts to make it easier for scientists to use, contribute to, and publish open software and data. ([slides](https://github.com/az-digitalag/organization/blob/master/presentations/20200111_PAG_LeBauer.pdf))

2. Tyson Swetnam presented “The Airborne Environmental Observations Laboratory for Unoccupied Systems (AEOLUS)” ([abstract](https://plan.core-apps.com/pag_2020/abstract/1ff1f7d3-b909-4da5-9180-e823311c25c8)) ([slides](https://gitpitch.com/tyson-swetnam/2020-01-11-PAG/master#/)). This included our work to on the [Drone Processing Pipeline](https://osf.io/xdkcy/) to support the data management lifecycle and scale it to leverage high performance computing resources. The talk presents scientific workflows as a “choose your own adventure” story - they need to be flexible enough to meet individual needs, but standardized enough to abstract complex software engineering. He also describes existing software as well as computing infrastructure available through [CyVerse](https://cyverse.org/) and NSF’s network of high performance computers [XSEDE](https://www.xsede.org/).  

3. Sateesh Peri presented “PhytoOracle: A Scalable, Modular Framework for Phenomics Data Processing and Trait Extraction.” ([abstract](https://plan.core-apps.com/pag_2020/abstract/fe6a83b2-61a4-404e-bf4f-b1760d0cc7d5)) This talk described a substantial effort by the Applied Concepts in Cyberinfrastructure class in Fall 2019 to re-architect the TERRA REF pipeline to make it more modular and scalable as well as easier for scientists to use and contribute to. Key features include the first use of new algorithm templates being developed by Chris Schnaufer in our group, as well as adoption of [Makeflow](http://ccl.cse.nd.edu/software/makeflow/) workflow engine and [Work Queue](http://ccl.cse.nd.edu/software/workqueue/) for scaling to high performance computers. Learn more about the class' software, PhytOracle, in the [GitHub repository](https://github.com/uacic/PhytoOracle) and [documentation](https://phytooracle.readthedocs.io/en/latest/) that showcase their impressive work. The architecture that they developed was quickly integrated into our Phenomics pipeline development work - re-factoring the software used to process data from the TERRA REF gantry system in Maricopa. And three students are continuing to contribute to this effort.

4. Anne Thessen presented “Predicting Phenotype from Multi-Scale Genomic and Environment Data using Neural Networks and Knowledge Graphs: An Introduction to the NSF GenoPhenoEnvo Project” ([abstract](https://plan.core-apps.com/pag_2020/abstract/f489aeb2-5b59-4a10-bf11-dfe5b4ebcd3e)) describing a project we are working on to develop a machine learning framework that can predict plant phenotypes across spatial, temporal, and taxonomic scales from genomics and environmental data. The first year focuses on using TERRA REF data and in the second year we will begin scaling up to use data from the National Ecological Observatory Network and the National Phenology Network. You can learn more about this work at our [GenoPhenoEnvo project website](https://genophenoenvo.github.io/).
