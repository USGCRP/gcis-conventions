# Table Conventions

## Appropriate Use Case

- The high level representation of array data.  
- They represent the Table objects in Reports.  
- We only create them for USGCRP publications.  
- We create them by hand.  

# Field Conventions

| Field | Description |
|-------|------------- | 
|**identifier**|Short identifier based on the title.|
|**ordinal**|The numeric position of this table within a chapter. Must start with a number, may contain numbers, letters, dashes, dots and underscores|
|**title**|The title of the table as it appears in the publication.|
|**caption**|The visible explanatory text that accompanies the array data in the publication.  When there is a difference in the caption between the print and online tables, we match the online table.|  
|**url**|Generally not used.  If the Table has a proper, stand alone landing page, it should go here.  |


## Provenance Conventions

As child:  
**prov:wasDerivedFrom**  

With very rare exceptions, not to be used on Tables, but rather their underlying Array.

**cito:cites**

If a cell in the array or a statement in the caption includes a citation, the table should use this semantic connection to link to the reference.

As parent:  
**cito:isCitedBy**  
**prov:wasDerivedFrom**  

These are used when future USGCRP publications cite or derive things from the table.  
We do not actively look for outside use of the table.  

## Relationship Conventions

**Chapter**

If the Table is within a chapter, this should be connected.  
If the Table is in a publication lacking chapters, this may be blank.  

**Report**

Should always be provided, linking to the containing publication.  

**Contributors**

To be filled in if specified in the Publication and we chose to do so on a Publication wide basis.

**Files**

Not used.

**gcmd_keywords**

Can be associated if used on a publication wide basis.  

**regions**

not implemeneted

**Array**

Every table should have at least one array.
