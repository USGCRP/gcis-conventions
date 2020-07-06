# Journal Conventions

## Appropriate Journal Use Case

Journals are generally populated automatically when Articles are imported from the EndNote.  
Some may be created by hand, in those same circumstances, when auto-creation fails.  

## Field Conventions

| Field | Description |
|-------|------------- | 
|**identifier**|This is based on the title.  When creating a journal, leave the identifier blank such that the system autocreates it without the articles.|  
|**title**|The title according to crossref.  Fallback to the title on the website or best available source.|
|**publisher**|Deprecated in favor of the Contributor relationship, role Publisher.  |
|**country**|Optional.  If filled in, use the country codes as they appear in our Countries table.  Fill in if this improves clarity.|
|**url**|We strongly want this filled in.  For defunct journals, point to the official archive website, if any.  Can be left blank if no such url is available.  |
|**notes**|Currently used to capture the provenance connection we can't capture semantically.  No other good use. Do not use.  |
|**print_issn**|We want to have at least one of the ISSNs.  If there is more than one print ISSN, use the first listed & functional ISSN.|
|**online_issn**| We want to have at least one of the ISSNs.  If there is more than one online ISSN, use the first listed & functional ISSN.|

## Provenance Conventions


## Relationship Conventions

**Article**

  - Journals should only be created when needed because of an Article being in GCIS.

**Contributors**

  - Every Journal should have a contributor Organization with role Publisher
  - If a Journal changes Publisher, and we have articles under both, we should update to have a Publisher and a 'Former Publisher'

**Files** 

An exemplar image of an issue of the Journal, pulled from their website.

**gcmd_keywords**

Not used on this object.

**regions**

Not yet implemented.

## Unresolved Conventions

### Provenance: Related Journals

We are debating the merits of a provenance connection between related journals (i.e. defunct & successor).
