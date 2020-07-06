# Book Conventions

## Appropriate Book Use Case

Books are not created by us directly, but rather as children publications for references.   
Reports may have ISBNs, and be published as physical books, but they still better fit as a `Report` object over a `Book` object.  

## Field Conventions

| Field | Description |
|-------|------------- | 
|**identifier** | Fine as UUID. [See default: UUID](./Defaults.md#UUID). GCIS will automatically generate one from a blank `identifier` field|
|**title**| The book title, as given by TSU. Checked against the WorldCat.|
|**isbn**| Required if the book has one. We prefer the thirteen digit one if it exists. Should be the one that links properly to WorldCat. We do not have a preference for ISBNs of different editions (e.g. hardcover vs paperback), so long as it is correct and matches our other metadata.|
|**year**| The publication year of the edition of the book matching the ISBN. If ISBN is not known, then the publication year of the first edition is preferred.|
|**publisher**|Going forward, deprecated. Use a contributor with role Publisher.|   
|**number_of_pages**|Imported from WorldCat. Not a priority if not available from WorldCat.|
|**url**| Official online published copy of the book is fine, if available. Use the publisher's webpage for this book. Imported from TSU or WorldCat. Research to find it otherwise.|
|**in_library**|**Deprecated.** | 
|**topic**| Imported from TSU or WorldCat. Not a priority to fill in otherwise.|  

## Provenance Conventions

Only `cito:isCitedBy` is used, created from the Reference.  
Nothing is created off of the book itself.

## Relationship Conventions

**Contributors**
  - The Publisher role is the first priority.  
  - Editors and authors roles are second priority.  
  - Other roles can be added as appropriate for each case  

**File**  
  - Can have a related file if available. Not a priority.

**gcmd_keywords**
  - not to be used for the moment. To be determined.
 
**Regions**
  - not to be used.
