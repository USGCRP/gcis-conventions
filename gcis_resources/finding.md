# Finding Conventions

## Use Case

In USGCRP Reports, every chapter has a "Key Message" - a short statement of fact with backing supporting evidence. Only used on USGCRP published reports, and only exists as a subobject.


## Field Breakdown

| Field | Description |
|-------|------------- | 
|**identifier** | Should follow the convention of:`Key-Finding-CH#-ORD`  `Key-Message-CH#-ORD`  The initial part of the identifier should match the naming of this object type for that report|
|**chapter_identifier** | The chapter, if any, that contains this finding.|
|**statement** | The shorter, headline sentence that conveys the key information.Filled in via data provided from TSU. Data contained within is provided by the authors following guidance.  HTML Formatting is supported.  Callouts to References should be done via their UUIDs, and captured within `<tbib>` tags.|
|**ordinal**|  The ordinal as specified in the actual report.|
|**report_identifier**|  The report that contains this finding.|
|**process** | Filled in via data provided from TSU. Data contained within is provided by the authors following guidance. HTML Formatting is supported. Callouts to References should be done via their UUIDs, and captured within `<tbib>` tags.|
|**evidence**  |Filled in via data provided from TSU. Data contained within is provided by the authors following guidance. HTML Formatting is supported. Callouts to References should be done via their UUIDs, and captured within `<tbib>` tags.|
|**uncertainties**| Filled in via data provided from TSU. Data contained within is provided by the authors following guidance. HTML Formatting is supported.  Callouts to References should be done via their UUIDs, and captured within `<tbib>` tags.|
|**confidence** | Filled in via data provided from TSU. Data contained within is provided by the authors following guidance. HTML Formatting is supported.  Callouts to References should be done via their UUIDs, and captured within `<tbib>` tags.|
|**url** | If there is a direct URL to the finding, add it here. Prefer not linking to the general parent page (aka the chapter). |

## Provenance Connections:

 **cito:cites** & **cito:isCitedBy**

 - The Finding cites its references
 - If future USGCRP product cite this Finding, it may have 'isCitedBy'

## Relationship Connections:

**Chapter**

If it is within a report chapter, this must be filled in.

**Report**

This must be filled in.

  
