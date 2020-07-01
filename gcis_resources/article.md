# Article Conventions

## Appropriate Use Case

The article resource type in GCIS is used to represent articles referenced in USGCRP reports. This means that each article in the GCIS is used as a reference in a USGCRP report.

## Identifier Convention

An article's [DOI](../external_conventions/doi.md) is used as the identifier when it is available.  
Acceptable fall-back identifiers we will use include [PMID](https://www.ncbi.nlm.nih.gov/pmc/pmctopmid/), [PMC](https://www.ncbi.nlm.nih.gov/pmc/pmctopmid/), and [CDC MMWR](https://www.cdc.gov/mmwr/about.html).

If the article doesn't have any of these external identifiers, we use the title, with hyphens between words, lowercase letters, no numbers. We do not remove any words.

**Examples:**
   * for an article having the doi of [10.1002/aqc.880](http://data.globalchange.gov/article/10.1002/aqc.880)
      * http://data.globalchange.gov/article/10.1002/aqc.880
   * for an article without a DOI, but has a PubMed ID of [pmid-22377962](https://data.globalchange.gov/article/pmid-22377962)
      * https://data.globalchange.gov/article/pmid-22377962
   *  since this article doesn't have a doi or other acceptable external identifier, we use the title.
      * http://data.globalchange.gov/article/resilience-adaptability-and-transformability-in-socialecological-systems
      * **Note:** this will be common practice for articles in law journals, which don't tend to have DOIs

## Primary Field Conventions
| Field | Description |
|-------|------------- | 
|**Title**|Title should match the exact Article title|
|**DOI**|The exact DOI, if one exists. Otherwise blank.|
|**Year**|The year the article was published, as in the year this volume of the journal came out.|
|**Notes**|Not In Use.  May be used in the future for extraordinary circumstances, i.e. journal retractions.|
|**Journal**|Should refer to the GCIS Journal entity corresponding to the article's Journal.Should never be blank.|
|**URL**|Should always be provided if we don't have a DOI.  Preferred to have regardless.  In the case of neither a DOI nor a URL existing, may be left blank.|
|**journal vol**|Which volume of the Journal this article was published from.| Sourced from crossref.org, not from the corresponding imported reference.|
|**journal pages** |Which pages of the journal this article occurs at.  Preferred to be a page range. Initial page is acceptable.  Sourced from crossref.org, not from the corresponding imported reference.|

## Provenance Conventions

- We relate articles to USGCRP produced publications only.  
- An article can be `cito:isCitedBy` a USGCRP publication.  
- An article can `cito:cites` a USGCRP publication.

## Relationship Conventions


### Contributors

We connect Persons & Organizations to Articles with the follow conventions:
  * **Role Types**
    * author is the assumed role
    * point of contact role is used for specified corresponding author
    * other roles are not used unless they are called out in the article
  * [sort key](https://github.com/USGCRP/gcis-conventions/blob/master/gcis_resources/Defaults.md#sort-key) should be used to match the article's order
 
In cases of articles with hundreds of authors, some editors, & a point of contact. Only editors & PoC are added.

### gcmd_keywords
Not to be used at this time.
### regions
Not to be used at this time.
### files
Not used on articles
