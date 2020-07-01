# Report Conventions

## Appropriate Use Case: 
Publications, both external publications (not published by USGCRP) and USGCRP publications, that have officially been released as reports, and that need to be uploaded to the GCIS database, are created as reports in the GCIS.

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

## Report Type

We use the type as named by the distributor.  
Default is `report`. 

## Contact Note / Email

We add the email for the USGCRP reports, and notes when available.

## Contributors

- Reports should have their contributors.  
- When possible, contributors should have the person and the organization, but Organization only is acceptable.  
- [Sort key](https://github.com/USGCRP/gcis-conventions/blob/master/gcis_resources/Defaults.md#sort-key) should be used to make the contributor order match the report.

## URL, DOI, or File

All reports should either have a `URL`, a `doi`, an associated `file` to download, or both.

## Title

Title is generally imported directly from TSU's EndNote. It should match the external title.

## Provenance Conventions:
- cito:cites
- cito:isCitedBy
- prov:wasDerivedFrom
- prov:wasInformedBy

# Indicator Conventions

## Identifier

Follows the [title](https://github.com/USGCRP/gcis-conventions/blob/master/gcis_resources/Defaults.md#title) process, with an added postfix of the year.

## Title 

Should match the published title of the Indicator, with an added prefix of `Indicator:`

## URL

Only the most recent year Indicator should have a URL.




             

