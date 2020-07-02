# Finding Conventions

## Use Case

What is a Finding?  
In USGCRP Reports, every chapter has a "Key Message" - a short statement of fact with backing supporting evidence.  
Only used on USGCRP published reports, and only exists as a subobject.

## TODO

 - Ask TSU for their guidance for the fields:
    + evidence
    + statement
    + process
    + uncertainty
    + confidence

## Field Breakdown

| Field | Description |
|-------|------------- | 
|**identifier** | <li>Should follow the convention of:`Key-Finding-CH#-ORD`  `Key-Message-CH#-ORD`  <li>The initial part of the identifier should match the naming of this object type for that report|
|**chapter_identifier** | <li>The chapter, if any, that contains this finding.|
|**statement** | <li>The shorter, headline sentence that conveys the key information.<li>Filled in via data provided from TSU. Data contained within is provided by the authors following guidance.  <li>HTML Formatting is supported.  <li>Callouts to References should be done via their UUIDs, and captured within `<tbib>` tags.|
|**ordinal**|  <li>The ordinal as specified in the actual report.|
|**report_identifier**|  <li>The report that contains this finding.|
|**process** | <li>Filled in via data provided from TSU. Data contained within is provided by the authors following guidance.  <li>HTML Formatting is supported. <li>Callouts to References should be done via their UUIDs, and captured within `<tbib>` tags.|
|**evidence**  |<li>Filled in via data provided from TSU. Data contained within is provided by the authors following guidance.  <li>HTML Formatting is supported. <li>Callouts to References should be done via their UUIDs, and captured within `<tbib>` tags.|
|**uncertainties**|  <li>Filled in via data provided from TSU. Data contained within is provided by the authors following guidance.  <li>HTML Formatting is supported.  <li>Callouts to References should be done via their UUIDs, and captured within `<tbib>` tags.|
|**confidence** | <li>Filled in via data provided from TSU. Data contained within is provided by the authors following guidance.  <li>HTML Formatting is supported.  <li>Callouts to References should be done via their UUIDs, and captured within `<tbib>` tags.|
|**url** | <li>If there is a direct URL to the finding, add it here.  <li>Prefer not linking to the general parent page (aka the chapter).  |

## Provenance Connections:

 **cito:cites** & **cito:isCitedBy**

 - The Finding cites its references
 - If future USGCRP product cite this Finding, it may have 'isCitedBy'

## Relationship Connections:

**Chapter**

If it is within a report chapter, this must be filled in.

**Report**

This must be filled in.

  
