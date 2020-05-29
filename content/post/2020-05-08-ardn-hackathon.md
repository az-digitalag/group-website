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

The first week of May, David and I participated in a hackathon on agricultural data formats. 
This event was part of a project called the Agricultural Research Data Network (ARDN), which was funded by a NIFA FACT grant (2019-67021-29921).
The project is unique in that the majority of work is done in bi-annual week-long hackathons. This was the second of six hackathons scheduled during the project. 
 This project is led by a team from the University of Florida's [department of Agricultural and Biological Engineering](https://abe.ufl.edu/people/), including Cheryl Porter and Gerrit Hoogenboom. 
 Cheryl and Gerrit are leaders in the Agricultural Model Intercomparison project, and have developed a common data format for agricultural models called [ACE](https://vest.agrisemantics.org/content/icasa-data-standards-agricultural-field-experiments-and-production) (AgMIP Crop Experiment data schema, Porter et al 2014).

The purpose of this ARDN project is to make a handful of agricultural datasets more *Findable, Accessible, Interoperable, and Reusable*, which is a broader movement referred to as [FAIR](https://www.force11.org/group/fairgroup/fairprinciples). Increasing how FAIR these datasets are should enable them to be used more broadly in crop modeling research. We are making the particular datasets in this project more *Findable* and *Accessible* by putting them on an easy-to-use platform called [Ag Data Commons](https://data.nal.usda.gov/), which is a data repository run by the USDA. The data are becoming more *Interoperable* and *Reusable* as we are converting them from their more diverse formats into a single compatible format. 

There are four initial datasets in the ARDN project, which are being converted to the ACE format and put on Ag Data Commons. Each comes from a different institution. A team at Michigan State is bringing data from [the Kellogg Biological Station LTER](http://www.kbs.msu.edu/), Lori Abenroth at Iowa State is contributing [the Corn CAP data](https://datateam.agron.iastate.edu/cscap/) (and already has [some of that data on ADC](https://data.nal.usda.gov/dataset/sustainable-corn-cap-research-data-usda-nifa-award-no-2011-68002-30190)), and the University of Georgia is contribuing variety trials from the University of Georgia. Our team at the University of Arizona is converting and registering data from the [TERRA REF](https://www.terraref.org/) highthroughput phenotyping dataset. 

Our group is focusing on converting the TERRA REF data that is accessible through the (plant) Breeder's API ([BrAPI](https://www.brapi.org/), Selby et al 2019) into the ACE format.
BrAPI is a specification for data from breeding trials that has been developed an implemented by dozens of crop breeding databases worldwide.
TERRA REF has implemented a BrAPI compliant interface in order to make these data more accessible and interoperable with data from the larger plant breeding community.
For this ARDN project, we are in the process of specifying how to translate the BrAPI version of the TERRA REF data to the ICASA format, which will then be put on Ag Data Commons.

We were lucky to have the BrAPI community coordinator, [Peter Selby](https://blogs.cornell.edu/robbinslab/people/), join us during the hackathon. One of our goals during the hackathon week was to improve some of [our TERRA REF BrAPI endpoints](https://github.com/terraref/brapi/) to be more easily translatable to the ACE format, which we are continuing to do as we move forward. This communication between the BrAPI and AgMIP communities will help inform future extensions of BrAPI to support more detailed geospatial, time series, and agronomic management data required by the agricultural modeling and high throughput phenotyping communities.  

Our larger goal is to enable interoperability among datasets that adhere to one or more data and metadata format conventions. By the conclusion of the ARDN project, our group will have enabled any BrAPI-compliant data source with the necessary minimum metadata to be easily converted to the ACE format. 
Similarly, there should be a clear path for translating data annotated with Ecological Metadata Language into the ACE format. 

The diagram below illustrates our idea:

![Diagram showing process of translating TERRA REF data into BrAPI and then ICASA](/post/2020-05-08-ardn-hackathon_files/ARDN_diagram.png)

Having more data in a common format will make it easier for the modeling community to use of the data that is so difficult to collect in the field. 
It will also enable synthesis across studies, including cross-site and cross-species analyses. 
To facilitate data harmonization, the UF team is building a tool that steps the user through how to convert tabular data to the ACE format; this tool is called VMapper [Cheryl: can we link to the Vmapper?].

Overall, the ARDN hackathon was a success.
All of the teams involved made substantial progress converting their data and learning about Ag Data Commons submissions. 
This event ended up being done entirely virtually; while this was very productive, we look forward to future in person hackathons that provide focus and interaction among teams that benefit this type of work. 
These types of interdisciplinary projects, involving domain scientists, computer scientists, and modelers, are always inspiring collaboration experiences. 


### References

Selby, Peter, et al. "BrAPI—an application programming interface for plant breeding applications." Bioinformatics 35.20 (2019): 4147-4155.

Porter, Cheryl H., et al. "Harmonization and translation of crop modeling data to ensure interoperability." Environmental modelling & software 62 (2014): 495-508.