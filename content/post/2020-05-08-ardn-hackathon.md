---
title: Hackathon For Building the Agricultural Research Data Network
authors: 
- Kristina Riemer, David LeBauer
date: '2020-05-08'
slug: ardn-hackathon
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

![Zoom Group Photo of Hackathon Attendees](/post/2020-05-08-ardn-hackathon_files/ARDN_team_2020.05.jpg)

The first week of May, David and I participated in a hackathon on agricultural data formats. This event was part of a project called the Agricultural Research Data Network (ARDN), which was funded by a NIFA FACT grant. This project is led by a team from the University of Florida's [department of Agricultural and Biological Engineering](https://abe.ufl.edu/people/), including Cheryl Porter and Gerrit Hoogenboom. 

The purpose of this ARDN project is to make a handful of agricultural datasets more *Findable, Accessible, Interoperable, and Reusable*, which is a broader movement referred to as [FAIR](https://www.force11.org/group/fairgroup/fairprinciples). Increasing how FAIR these datasets are should enable them to be used more broadly in crop modeling research. We are making the particular datasets in this project more *Findable* and *Accessible* by putting them on an easy-to-use platform called [Ag Data Commons](https://data.nal.usda.gov/), which is a data repository run by the USDA. The data are becoming more *Interoperable* and *Reusable* as we are converting them from their more diverse formats into a single compatible format, specifically [the AgMIP ICASA standard](https://vest.agrisemantics.org/content/icasa-data-standards-agricultural-field-experiments-and-production). 

There are four initial datasets in the ARDN project, which are being converted to the ICASA format and put on Ag Data Commons. Each comes from a different institution. A team at Michigan State is bringing data from [the Kellogg Biological Station LTER](http://www.kbs.msu.edu/), Lori Abenroth at Iowa State is contributing [the Corn CAP data](https://datateam.agron.iastate.edu/cscap/) (and already has [some of that data on ADC](https://data.nal.usda.gov/dataset/sustainable-corn-cap-research-data-usda-nifa-award-no-2011-68002-30190)), and the University of Georgia is contribuing the xxx datasets. Our team at the University of Arizona is converting and registering our highthroughput phenotyping crop dataset [TERRA REF](https://www.terraref.org/). 

We are specifically using a subset of TERRA REF data that is accessed from an API called the Plant Breeding API ([BrAPI](https://www.brapi.org/)). TERRA REF was made compliant with BrAPI so that it is more accessible to the plant breeding community. For this ARDN project, we are in the process of specifying how to translate the BrAPI version of the TERRA REF data to the ICASA format, which will then be put on Ag Data Commons. The diagram below shows this conceptual flow. 

![Diagram showing process of translating TERRA REF data into BrAPI and then ICASA](/post/2020-05-08-ardn-hackathon_files/ARDN_diagram.png)

We were lucky to have the BrAPI community coordinator, [Peter Selby](https://blogs.cornell.edu/robbinslab/people/), join us during the hackathon. One of our goals during the hackathon week was to improve some of [our TERRA REF BrAPI endpoints](https://github.com/terraref/brapi/) to be more easily translatable to the ICASA format, which we are continuing to do as we move forward. Ideally by the end of the ARDN project, we will have enabled any other BrAPI-compliant dataset to be easily converted to the ICASA format, with TERRA REF as a useful example of this. 

Other long-term goals for ARDN include faciliating the conversion and addition of other datasets. Though it is not expected that all possible datasets should go through this process, having more similarly useful data harmonized in this manner will make it easier to model on broader scales and build tools for this modeling. This can also result in new collaborations and research avenues forming. To make this process easier for additional datasets, the UF folks are building a tool that steps the user through how to convert tabular data to the ICASA format; this tool is called VMapper. We also hope to include EML into this work, which could result in expansion to datasets such as those stored at [DataONE](https://www.dataone.org/). 

Overall, the ARDN hackathon was a success. All of the teams involved made substantial progress converting their data and learning about Ag Data Commons submissions. This event ended up being done entirely virtually, which was still a very productive method, though in some ways more tiring than an in-person meeting would have been due to different types of distractions. These types of interdisciplinary projects, involving domain scientists, computer scientists, and modelers, are always inspiring collaboration experiences. 
