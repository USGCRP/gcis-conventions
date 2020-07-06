# Web Page Conventions

## Appropriate Web Page Use Case

- Web pages are brought in via citations but Reports, Figures, Images, etc.  
- Web tools are categorized as web pages.  

### Distinguishing Webpages from Datasets

After web page type references are imported, a QA should be done before production release to check if any would be better categorized as datasets.

### Field Conventions

| Field | Description |
|-------|------------- | 
|**identifier**| Fine as UUID.  [See default: UUID](./Defaults.md#UUID). GCIS will automatically generate one from a blank `identifier` field|
|**url**|  The full url, not including any parameters.  Parameters should be collected on either the `activity` or `reference`s as appropriate.|
|**title**| Whatever the Reference names the URL  otherwise as stated on the webpage itself  correct as of the creation of the object.|
|**access_date**|  *deprecated*. The access date for this webpage. Should not be used, as we have unique URL requirement.  A access date should go on either the Reference object (e.g. if this is a referenced publication) or an Activity object (e.g. if this cited on a Figure)|

## Provenance Conventions

- Webpages are valid to be `cito:CitedBy`, usually by Figures or Images.  
- They do not use `cito:Cites`, as they are not USGCRP products.  

## Relationship Conventions

**Contributors**

 - Webpages often have a host, and may have authors, as appropriate.

**File**

 - Not used on Webpages.

**gcmd_keywords**
 - not to be used for the moment. To be determined.
 
**regions**
 - not to be used.
