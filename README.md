# The Global Change Information System: an overview of its Data Model and Metadata Conventions v2.0


## Summary of updates to the GCIS

The following key changes have been  made to the latest version of the Global Change Information System (GCIS):
- Data Export Formats: The GCIS no longer leverages semantic formats -- [Turtle](https://www.w3.org/TR/turtle/), [N-Triples](https://www.w3.org/TR/n-triples/), [JSON Triples](https://www.w3.org/wiki/JSON_Triple_Sets), [RDF+XML](https://www.w3.org/TR/rdf-syntax-grammar/), and [RDF+JSON](https://www.w3.org/TR/rdf-json/) -- nor rely on visual representations with [Graphviz]() and [SVG](). 
- The GCIS has integrated two new external resources:

| Resource                               | Application                                                                                                                                                                                                                                                        |
|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [ROR](https://ror.org/)               | Provides unique and usable identifiers for GCIS Organizations. Organizations are now mapped to external  [ROR](https://ror.org/) identifiers through the [Lexicon](https://github.com/USGCRP/gcis-conventions/blob/v2.0.0/gcis_resources/lexicon.md) data model. |
| [Crossref](https://www.crossref.org/) | Displays publications that cite a USGCRP report on the report’s index page. Currently used for NCA4 only.                                                                                                                                                          |

- The GCIS now reflects several minor changes to resource field names, including an overhaul of the Indicator resource type: previously treated as a Report subset, it is now rightly regarded as a [Figure](https://github.com/USGCRP/gcis-conventions/blob/v2.0.0/gcis_resources/figure.md) type.




## Introduction

With over [22,000 people](https://data.globalchange.gov/person), [7,000 articles](https://data.globalchange.gov/article), [12,000 organizations](https://data.globalchange.gov/organization), [3,000 datasets](https://data.globalchange.gov/dataset), and much more, the [Global Change Information System](https://data.globalchange.gov/), or GCIS, catalogs a copious amount of information and metadata for the U.S. Global Change Research Program (USGCRP). Metadata contained in the system include the names of USGCRP report authors and their affiliations, report figures and images, datasets, and a substantial list of referenced documents, such as the publications of the Intergovernmental Panel on Climate Change. These are either relationally or semantically linked with one another to improve the traceability of climate information and data provenance, thereby bolstering the overall utility of the GCIS. As a prime access point to U.S federal assessments on climate change, reports, and tools produced by the USGCRP – including the native data that underpins these resources – the GCIS is an important initiative for robust Global Change research.  

Given this brief description of the GCIS, it is imperative that the system make use of existing and highly regarded metadata standards and conventions where possible. This document aims to describe the current GCIS data model, as well as highlight all the conventions and standards deployed in the system. 






## Sections

[Metadata Standards](metadata_standards)  
What standards we adhere to and how.

[GCIS Data Model](data_model)  
GCIS data structure, entities and relationships. 

[GCIS Resources](gcis_resources)  
The conventions we have created for the GCIS resources, such as Reports or Figures.  

[External Conventions](external_conventions)  
How we use external identifiers, such as DOIs or UUIDs.  



