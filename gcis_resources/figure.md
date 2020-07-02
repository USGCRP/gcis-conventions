# Figure Conventions

## Appropriate Figure Use Case

Figures should be created for USGCRP Publications.  
They are generally created automatically via a syncronizing with the TSU Resources Metadata.  

In the case of supported non-USGCRP Publications, Figures may be created if the publishing entity provides the information.

## Field Conventions

| Field | Description |
|-------|-------------| 
|**identifier**|<li> The title of the figure with hyphens.  <li> May differ if the figure is renamed late in the report process. <li> Generally, we write "US" instead of "United-States"
|**chapter_identifier**|<li> The associated chapter identifier inside the report, if any, associated with the figure.|
|**title**|<li> The title of the Figure as set by TSU.  <li> In the case of Figures not from TSU, the title as it appears in the report.|
|**caption**|<li> Any text appearing alongside the figure.|
|**attributes**| <li> _deprecated_. <li> Unknown use. Not filled in anywhere.
|**time_start** **time_end**|<li> The start and end of the temporal extent represented by this figure.  <li> We _prefer_ to have these on the image rather than the figure.|
|**lat_max** **lat_min** **lon_max** **lon_min**|<li> The nothernmost/southmost latitude & eastmost/westmost longitudes in the bounding box for this figure. <li> We _prefer_ to have these on the image rather than the figure.<li> Future development: https://en.wikipedia.org/wiki/Well-known_text  |
|**usage_limits**| <li> Copyright restrictions describing how this figure may be used by the general public.  <li> Historically this has not been filled in properly. <li>Needs to come from TSU, but should not be filled in from their usage limits, but rather whether we created it or not.<li> For non-TSU figures, fill in accordingly.    |
|**submission_dt**|<li> Currently, we think this is the last update before submission.  <li> Followup needed. <li>Final determination to be made after conversation with TSU.  |
|**create_dt**|<li> Currently, we think this is the initial creation in TSU's system.  <li> Follow-up needed.<li> Final determination to be made after conversation with TSU.|  
|**source_citation**|<li> If this isn't an original creation, the citation to that.<li> Follow-up: should this be captured in provenance?|
|**ordinal**|<li> The internal chapter or report numbering <li> (alphanumeric)|
|**report_identifier**|<li> The associated report identifier the figure.|
|**url**|<li> Direct URL to the Figure landing page in the associated report, if any.  |
|**_origination**|<li> Internal field to hold data needed by TSU for presetnation of report websites. <li> Eventually to be phased out via Activity & TSU Sync updates.|

## Provenance Conventions

**cito:cites**

  - Figures can cite their sources

**cito:isCitedBy**

  - If the Figure has been cited in a future USGCRP publication, it may be marked as isCitedBy

**prov:wasGeneratedBy**, **prov:wasDerivedFrom**, **prov:wasInformedBy**

  - These provenence relationships would be better placed on the Image associated with a Figure, rather than on the Figure itself.

## Relationship Conventions

**Image**

  - All Figures should have an Image.
    - A Figure should have an Image for each logical subpanel within the figure. 
    - When a logical subdivision of the Figure is unavailable, a single backing Image is acceptable.
  - For when the TSU creates the Figures & Images, the Image subobjects are expected to have proper context and not just be cropped subsections of the Figure.

**Report**

  - Figures must belong to a Report or Indicator.

**Chapter**

  - Figures may belong to a Chapter, if the Report is broken into Chapters and the Figure is within them.

**Contributors**

 - All Figures should have a Point of Contact
 - Figures may have authors, editors, or other contributors depending on the associated Assessment.

**regions**

  - Not yet implemented.

**gcmd_keywords**

  - On a case by case basis for the parent report, we may assign GCMD keywords to the Figure.

**File**

  - All figures should have a high resolution image file associated with it. 
  - Preference for PNG for vector-like graphics and JPG for photo-like graphics.
