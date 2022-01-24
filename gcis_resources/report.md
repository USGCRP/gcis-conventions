# Report Conventions

## Appropriate Use Case: 
Publications, both external publications (not published by USGCRP) and USGCRP publications, that have officially been released as reports, and that need to be uploaded to the GCIS database, are created as reports in the GCIS.
## Primary Field Conventions

| Field | Description |
|-------|------------- |
|**Identifier**|The title of the report with dashes in place of the spaces.|
|**Title**|Title is generally imported directly from TSU's EndNote. It should match the external title.|
|**URL**|Should always be provided if we don't have a DOI. Preferred to have regardless. In the case of neither a DOI nor a URL existing, may be left blank.|
|**DOI**|The exact DOI, if one exists. Otherwise blank.|
|**Summary**|A brief summary of the report.|
|**Publication Year**|The year of publication as indicated on the report's official landing page.|
|**In library**|Whether or not this report is available in the USGCRP Resources Library.|
|**Report Type**|We use the type as named by the distributor. Default is “report”.|
|**Frequency**|Captures how often the report would be released, if the report is meant to be released periodically.|
|**Public**|Indicates that the report is publicly readable.|
|**Topic**|A brief free form comma-separated list of topics associated with the report.|
|**Contact Note**|A note about contacting someone about the report. Phrases [in brackets] in the note will become links to the contact email. Added when this is available.|
|**Contact Email**|A contact email address for the report. Added when this is available.|

## Identifier Convention

 - If the distributor website has an official identifier, we use that.  
   - US Forest Service Report "Pacific Northwest Research Station General Technical Report 255" with internal identifier `PNW-GTR-855`
   - `http://data.globalchange.gov/report/usfs-pnw-gtr-855` 
 - If there is a widely accepted identifier, we use that.  
   - USGCRP's Third National Climate Assessment is known as NCA3
   - `http://data.globalchange.gov/report/nca3`
 - If we have to create it: `Distributor abbreviation`-`hyphenated-title`-`version, if known, otherwise year`
   - This is an ACWI report called "A National Framework for Ground-Water Modeling in the U.S." which was published in 2013.
   - `http://data.globalchange.gov/report/acwi-nationalframework-2013` 


## Contributors

- Reports should have their contributors.  
- When possible, contributors should have the person and the organization, but Organization only is acceptable.  
- [Sort key](https://github.com/USGCRP/gcis-conventions/blob/master/gcis_resources/Defaults.md#sort-key) should be used to make the contributor order match the report.

## File

All reports should either have a `URL`, a `doi`, an associated `file` to download, or both.

## Provenance Conventions:
- cito:cites
- cito:isCitedBy
- prov:wasDerivedFrom
- prov:wasInformedBy

# Additional Notes on Reports:
- Crossref integration: GCIS currently displays cited-by publications via [Crossref cited-by](https://www.crossref.org/services/cited-by/) service.
- Although indicators have been migrated to figures and are no longer reports, they sit under an empty parent report for each year called “indicators-{year}” . For example, visiting ‘/report/indicators-2018/’ will show you a list of all indicators (figures) for the year 2018.







             

