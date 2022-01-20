# Dataset Conventions

## Appropriate Dataset Use Case

Datasets are created in GCIS when cited by Reports, Figures, Tables, etc.  
A dataset should be unique per version.  
Dataset has many extraneous or problamatic fields. Create with caution.

## Field Conventions

### Valid Fields

| Field | Description |
|-------|------------- | 
|**identifier**|An external ID is preferred *if sufficiently unique*. Data.gov is preferred as an external ID. DOI is also acceptable. Identifier must be unique for *this version* of the dataset. If no acceptable external ID, `org_name` + `dataset_name` + `version` In version, `.` become `_`If no version, `org_name` + `dataset_name` + `publication_year`
|**name**| Use the same name as the external source.|
|**version**|The external version, if any. Follows their convention.|
|**description**| Any available description from the landing page or website of organization. May be shortened.|
|**native_id**|The external id, if any. The identifier for this dataset given by the producer or archive for the dataset.|
|**url**| A URL for a landing page. Probably can't be guaranteed unique.||
|**doi**| The DOI for this dataset, if any. Probably can't be guaranteed unique.|
|**release_dt**| The date on which this version of this dataset was released.|
|**publication_year**| The date on which this dataset was initially published, regardless of version.|
|**description_attribution**| A URL which contains the description of this dataset given in the description field. If same as URL, duplicate URL here.|
|**report_id**|the GCIS id of the report this resource belongs to.|
|**chapter_id**|the GCIS id of the report this resource belongs to.|




### Soft Deprecated Fields

These fields have more to do with the dataset itself, and belong with the owner of the dataset not with USGCRP's system.

 - type                   
 - data_qualifier         
 - spatial_ref_sys        
 - cite_metadata          
 - scope                  
 - processing_level       
 - spatial_res            

### Hard Deprecated Fields

These fields could go on an associated Activity, but would be actively harmful on the Dataset:

 - access_dt
 - scale

If a subset of the data was used, these fields may be relevant but belong on the Activity not the Dataset.

 - start_time             
 - end_time               
 - lat_min                
 - lat_max                
 - lon_min                
 - lon_max  
 - spatial_extent         
 - temporal_extent        
 - vertical_extent      
 
These fields should not be used:

 - attributes             
 - variables  

## Provenance Conventions

Datasets use `prov:wasDerivedFrom`, where a figure "prov:wasDerivedFrom" a dataset, through an activity

## Relationship Conventions

**Contributors**
 - Datasets should have their owner organiation linked to them via a contributor.
 - Normally via the `data_archive` role.

**Files**
 - Historically Datasets have sometimes had a jpg associated with them. 
 - Not required

**Report**
 - Dataset  may belong to a Report or Indicator. 
 
**Chapter**
 - Dataset  may belong to a Chapter, if the Report is broken into Chapters and the dataset  is within them. 

**GCMD_ Keywords**
 - not to be used for the moment. To be determined.
 
**Regions**
 - not to be used.
