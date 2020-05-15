---
title: Hackathon to Put TERRA REF on BrAPI
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

## Draft

The first week of May, David and I participated in a hackathon on agricultural data formats. This event was part of a project called the Agricultural Research Data Network (ARDN), which was funded by a NIFA FACT grant. This project is led by a team at the University of Florida, including Cheryl Porter and Gerrit Hoogenboom. 

The purpose of this ARDN project is to make a handful of agricultural datasets more Findable, Accessible, Interoperable, and Reusable, which is a broader movement referred to as [FAIR](https://www.force11.org/group/fairgroup/fairprinciples). By having these datasets more FAIR should enable them to be used more broadly in crop modeling. For ARDN, we are making these data more Findable and Accessible by putting them on an easy-to-use platform called [Ag Data Commons](https://data.nal.usda.gov/), which is a data repository run by the USDA. The data are becoming more Interoperable and Reusable as we are converting them from their more diverse formats into a compatible format, specifically AgMIP/ICASA. 

There are four datasets that we are currently converting to this format and putting on Ag Data Commons, each coming from a different institution. A team at Michigan State is bringing data from their Kellogg Biological Station LTER, Lori Abenroth at Iowa State is contributing the Corn CAP dataset, and the University of Georgia is contribuing the xxx datasets. Us at the University of Arizona are converting our highthroughput phenotyping crop dataset TERRA REF. 

We are specifically using a subset of TERRA REF data that is accessed from an API called the Plant Breeding API ([BrAPI](https://www.brapi.org/)). The data were made compliant with BrAPI to make it more accessible to the plant breeding community. For this ARDN project, we are in the process of specifying how to translate the BrAPI version of the TERRA REF data to the ICASA format, which will then be put on Ag Data Commons. See the diagram for this. We were lucky to have the BrAPI community coordinator, Peter Selby, join us for some of the hackathon. Part of our work during that hackathon was to improve some of our TERRA REF BrAPI endpoints to be more easily translatable. We have future work to do on this task. One of the end goals of this process is to enable any other BrAPI-compliant datasets to be able to be easily converted to this ICASA format, just like TERRA REF. 

![Diagram showing process of translating TERRA REF data into BrAPI and then ICASA](/post/2020-05-08-ardn-hackathon_files/ARDN_diagram.png)

For other long-term goals for ARDN, the plan is to expand even further to other datasets. Though there is no expectation that all or most possible datasets to be converted to this format and put in the repository, having a decent number of similar dataset harmonized in this manner will make it much easier to build tools that model all of the data. This process also can bring together collaborators who might not have otherwise. For ARDN, the UF folks are building a tool called the VMapper that will make it easier to convert tabular data to the ICASA format. We also hope to make EML metadata convertible, which could in datasets such as those at DataONE with EML to be put into ARDN. 

Overall, the hackathon for the ARDN was a success. All the teams made a lot of progress converting their data and learning about Ag Data Commons submissions. This event ended up being done entirely virtually, which was still a very productive method though in some ways more tiring than an in-person meeting would have been due to different types of distractions. These sorts of interdisciplinary projects, involving domain scientists, computer scientists, modelers, are always inspiring collaboration experiences. 
