# Region Conventions

## Use Case

- The Regions resource type in GCIS represents the geographical regions described in USGCRP reports.
  

## Field Conventions

| Field | Description |
|-------|------------- | 
|**identifier**| A simplified version of the label with dashes.  In the future, we would like to change this to be a UUID to avoid too specific or broad naming.|
|**label**| Should match the most recent NCA report specified name of the region.  If no region, should match governmental name.  |
|**description**|  Ideally, taken from the text of the report.  At a minimum, a list of the governmental boundaries contained.  |



## Provenance Conventions

none


## Relationships

`publication`  
Used to connect reports, chapters, figures, findings, and tables to region(s).

