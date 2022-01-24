# Organization Conventions
## Appropriate Use Case: 
Organization objects capture the affiliations of “people” in GCIS. Ideally, each “person” in GCIS should have an affiliation. Having affiliations in GCIS improves provenance tracing.

## Field Conventions

| Field | Description |
|-------|------------- |
|**Identifier**|Organization name separated by hyphens. To denote divisions or offices within a larger entity, begin with the larger entity. Spell out names of agencies and universities in their entirety.|
|**Name**| The Organization's name. Spell out entire organization name, e.g. "National Oceanic and Atmospheric Administration". Use official name where at all possible, even where it may differ from the entry in a publication.|
|**Organization Type**|The type of organization. For example, Federal Organization, Research Organization, Commercial Organization, Academic Organization, and so on.|
|**URL**|Direct link to the Organization's landing page.|
|**Country**|The country within which the organization's primary HQ is located.|
|**International**|Flag indicating a multinational organization with HQs in multiple countries.|

## Identifier Convention

[See default: Title](./Defaults.md#Title)

- Organization name separated by hyphens.  
- To denote divisions or offices within a larger entity, begin with the larger entity. Spell out names of agencies and universities in their entirety.  

## Provenance Conventions: 
None

## Relationship Conventions:
- University of X at Y predecessor of University of X; (implies that former univ became latter one)
- University of X at Y branch of University System of Y; (implies former univ part of a univ system)
- University of X branch of University System of Y (implies newer univ part of that same system)
- Clearly this can be extended to offices, etc. Also as a corollary if in changing names the university changed systems, we'd clearly adjust the relationship accordingly. Wikipedia can be a huge help here.
- Since we associate people and organizations through publications. We use what is mentioned in the publication even if the affiliation has since changed. For example, we keep "National Climatic Data Center" even though it is now the "National Centers for Environmental Information." Since it was NCDC at the time of the publication, we keep it as such and employ the methodology used above. As such, if a web page URL is the same as that in a previous publication but now includes the "National Centers for Environmental Information" banner, we use NCDC in-lieu of NCEI if that is what the author would have seen at the time it was cited.
- If an organization relationship changes, do not revise. Simply update with the new relationship, keeping the older one.
- An organization is linked to an external identifier by [ROR](https://ror.org/about) through the [Lexicon](https://github.com/USGCRP/gcis-conventions/blob/v2.0.0/gcis_resources/lexicon.md) data model.


