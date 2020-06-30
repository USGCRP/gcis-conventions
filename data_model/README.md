## The GCIS Data Model
Global change information in the GCIS is structured using the GCIS data model. This data model represents relationships and entities (publications or resources) such as reports, report chapters, figures, images, tables, bibliographic entries, organizations, and people. These entities will, heretofore, be referred to as “resources”, in accordance with GCIS parlance.

## GCIS Resources:
The terminology below describes the resources represented in the GCIS :


| Resource  | Definition |
| ------------- | ------------- |
| Activity  | A description of the process used to construct a publication. Examples include: [063fd83f-nca3-maurer-r201304-process](https://data.globalchange.gov/activity/063fd83f-nca3-maurer-r201304-process).
|Article|An independent story in a journal, book, or other published material. In GCIS, an article has a DOI (if available), like [10.1002/grl.50527](https://data.globalchange.gov/article/10.1002/grl.50527), which is used to uniquely identify it.| 
| Book |  A long-form publication, generally centered around one particular topic. In GCIS, books are cataloged using UUIDs, though ISBN numbers are also listed. Examples include : [Water Is for Fighting Over and Other Myths about Water in the West](https://data.globalchange.gov/book/water-is-fighting-over-other-myths-about-water-west), [6d3eb0d6-568a-40d3-9b10-393f943038da](https://data.globalchange.gov/book/6d3eb0d6-568a-40d3-9b10-393f943038da). |
|Chapter| Used to separate reports into smaller, more subject-intensive sections. In GCIS, chapters feature a unique mnemonic identifier and possibly a number. Some chapters, like an appendix, do not have a number. Chapters may have figures, tables, findings, and references associated with them. Chapters can also have distinctive Contributors to their parent Report. An example is NCA4’s [Chapter 4 : Energy Supply, Delivery, and Demand](https://data.globalchange.gov/report/nca4/chapter/energy-supply-delivery-and-demand).|
|Contributor|A person or organization that creates information (usually a figure or image) listed in GCIS. Analogous to Author records linked to publications. A few examples of Contributor role  types can be found [here](https://data.globalchange.gov/role_type).|
|Dataset|A collection of data pertaining to a specific subject. Datasets are considered a type of publication. In GCIS, a dataset is given a unique mnemonic identifier, such as [nca3-ncep-ncar-r1](https://data.globalchange.gov/dataset/ncep-ncar-reanalysis-1).|
|Figure|A visual representation (e.g., a graph, map, photograph, diagram, chart, or a satellite image) referenced in the text. It may be composed of one or more images. Example:  [observed-us-temperature-change](https://data.globalchange.gov/report/nca3/figure/observed-us-temperature-change).|
|Finding|A major conclusion or discovery garnered from the scientific evidence presented in a report. Has a statement as well as phrases and bibliographic references describing the confidence level, uncertainties, and evidence for that finding. Example: [global-climate-is-changing](https://data.globalchange.gov/report/nca3/chapter/our-changing-climate/finding/global-climate-is-changing).|
|Image| The unique graphic used to create a figure. One or more images make a figure. Example: [1f5a3cdd-fc45-403e-bf11-d1772005b430](https://data.globalchange.gov/image/1f5a3cdd-fc45-403e-bf11-d1772005b430).|
|Instrument|A measuring apparatus. Often associated with one or more platforms via instrument instances. Example: [poseidon-2](https://data.globalchange.gov/instrument/poseidon-2).|
|Instrument Instance|A platform/instrument combination. It may be associated with one or more datasets. Example: [jason-1/poseidon-2](https://data.globalchange.gov/platform/jason-1/instrument/poseidon-2).|
|Journals|A publication containing a collection of articles, original research, and conclusions. Generally shorter than a book, peer-reviewed, and released in multiple volumes or periodicals. In GCIS, a journal may have a print and online ISSN, and is uniquely identified within GCIS using a mnemonic identifier (such as climatic-change). Example: [Biogeochemistry](https://data.globalchange.gov/journal/biogeochemistry).|
|Model|A simulation or projection based on previously gathered data. Models are used to simulate climate systems and create model runs. Example: [ccsm3](https://data.globalchange.gov/model/ccsm3).|
|Model Run|A unique piece of data ascertained by combining a model, scenario, time range, time resolution, and sequence number. 
|Organization| A group, such as an institution, agency, or NGO. In GCIS, organizations are uniquely identified by mnemonic identifiers. Example: [us-global-change-research-program](https://data.globalchange.gov/organization/us-global-change-research-program).|
|Person|Individuals associated with global change research. In GCIS, they are uniquely identified by numeric identifiers. Example: [person/16009](https://data.globalchange.gov/person/16009).|
|Platform|A host for information gathering tools/instruments. May host one or more instruments. Example: [Terra](https://data.globalchange.gov/platform/terra).|
|Project|Initiatives led by an organization to generate models and eventually reach conclusions. Example: [cmip3](https://data.globalchange.gov/project/cmip3).|
|Publication|A report-specific resource (such as a chapter, figure, finding, or table), or a non-report-specific resource (such as a journal, article, image, web page, book, or dataset).|
|Reference|A bibliographic entry or citation pointing to a publication, such as an article, web page, or book. In a report, a reference may appear in a chapter, figure, finding or table. References are labeled with a universally unique identifier (UUID). Example: [0006123e-10a3-4501-a89c-95a7921a9c3d](https://data.globalchange.gov/reference/0006123e-10a3-4501-a89c-95a7921a9c3d).|
|Region|An area separated by its climate, geographic makeup, or another identifying factor. Example: [alaska-us](https://data.globalchange.gov/region/alaska-us)|
|Report|An authored compilation of information on a particular subject. May contain chapters, figures, tables, findings, and references. Example: [NCA3](https://data.globalchange.gov/report/nca3) and [NCA4](https://data.globalchange.gov/report/nca4).|
|Scenario|A set of assumptions used to help understand potential future conditions. Example: [rcp_2_6](https://data.globalchange.gov/scenario/rcp_2_6)|
|Table|An organized list referenced in the text. Often embedded in a report. Example: [list-us-droughts](https://data.globalchange.gov/report/climate-science-special-report/chapter/drought-floods-hydrology/table/list-us-droughts)|
|Web Page|A single page of a greater website. In GCIS, a web page is assigned a UUID, like [26625ddf-dd19-4dd1-a35d-33c68c5b2d6e](https://data.globalchange.gov/webpage/26625ddf-dd19-4dd1-a35d-33c68c5b2d6e), to identify its state at a particular point in time.|  


Climate Science is a complex discipline. Given the amount of data generation and data processing involved, and the use of climate science data in critical decision making, traceable provenance becomes invaluable. The GCIS adopts both a relational model and a semantic model, to maintain traceable provenance for the resources it catalogs. 

![Figure 1](https://github.com/USGCRP/gcis-conventions/blob/v1.0.1/data_model/image2.png) 

**Figure 1**: The GCIS “traceable accounts” model. Each step in this chain is an additional layer of reproducibility, but also a significant increase in the difficulty of capturing and curating.


### Relational Model:
The relational model used by GCIS captures one-to-many, many-to-many, and many-to-one relationships between the resources listed above. Journals have many articles, reports have many figures, findings, tables, and chapters. The relationship between images and figures, is many-to-many, as is the relationship between resources or publications of any type  and contributors. 

![Figure 2](https://github.com/USGCRP/gcis-conventions/blob/v1.0.1/data_model/image5.png)
**Figure 2**: A representation of the GCIS relational model.

### Semantic Model:

Resources may also be related to each other, and in this case, the relationship between two resources can be annotated with a term from a semantic vocabulary. Furthermore, the relationship may have an “activity” associated with it. All GCIS resources have representations in Turtle (a semantic format for storing data). The GCIS vocabulary is defined in the GCIS ontology. Many other ontologies are used including, most notably PROV. The entity-activity-agent model of PROV has been applied to the GCIS through the use of resources, activities, and contributors.

![Figure 3](https://github.com/USGCRP/gcis-conventions/blob/v1.0.1/data_model/image31.png)

**Figure 3**: A representation of the GCIS semantic model. 

As illustrated above, the GCIS data model leverages widely recognized conventions and standards. Almost every GCIS resource conforms to existing international standards. However, in unique instances where established conventions are non-existent, the GCIS team develops its own conventions.



