# Organization Conventions
## Appropriate Use Case: 
Organization objects capture the affiliations of “people” in GCIS. Ideally, each “person” in GCIS should have an affiliation. Having affiliations in GCIS improves provenance tracing.
## Identifier Convention

[See default: Title](./Defaults.md#Title)

Organization name separated by hyphens.  
To denote divisions or offices within a larger entity, begin with the larger entity. Spell out names of agencies and universities in their entirety.  

**Examples:**
  * "Duke University Nicholas School of the Environment" or "Nicholas School of the Environment at Duke University"
    * `https://data.globalchange.gov/organization/duke-university-nicholas-school-environment`
  * "The Office of Air and Radiation in the EPA" or "EPA's Air and Radiation Office"
    * `http://data.globalchange.gov/organization/us-environmental-protection-agency-office-air-radiation for`
  * "the Pacific Northwest Research Station" or "USFS Pacific Northwest Research Station"
    * `http://data.globalchange.gov/organization/us-forest-service-pacific-northwest-research-station`
  * NOAA  
    * `http://data.globalchange.gov/organization/national-oceanic-atmospheric-administration`

# Adding organizations to GCIS
* identifier: see page called Identifier conventions
* name: spell out entire organization name, e.g. "National Oceanic and Atmospheric Administration."  Use official name where at all possible, even where it may differ from the entry in a publication.  e.g.,
   * University of Maryland, College Park                             # for the University of Maryland (only if referring to main campus)
   * Indiana University Bloomington                                      # for "University of Indiana" or "Indiana University" (for main Bloomington campus only)
   * The University of Arizona                                               # for "University of Arizona#" or "Arizona University."
   * National Oceanic and Atmospheric Administration        for NOAA
   * U.S. Environmental Protection Agency Office of Water  # for EPA Office of Water, EPA's Office of Water, or US EPA Water Office
   * Stinger Ghaffarian Technologies                                     # for SGT, Inc.
   * Science Systems and Applications, Inc.                          # for SSAI
   * Virginia Polytechnic and State University                         # for Virginia Tech
   * Georgia Institute of Technology                                       # for Georgia Tech
   * University of California, Los Angeles                               # for UCLA, or "University of California Los Angeles"
* organization type:
   * "academic" = degree-granting e.g. a university or department
   * "research" = non-degree granting research e.g. a university research center, consulting group, etc.
   * "city" = self-explanatory, e.g. a municipality's water department
   * "commercial" = profit company
   * "consortium" - self-explanatory.  Examples include the University Corporation for Atmospheric Research
   * "county" - self-explanatory
   * "federal" - self-explanatory
   * "federal - managed academic" - a Federal program managed by an academic entity.  Many DOE National Laboratories are examples as they are run by the University of California System.
   * "federal - managed private" - a Federal office managed by a private company, usually a contractor.  The USGCRP NCO is one-such example, although USGCRP proper is simply "Federal."
   * "federal corporation" - don't know
   * "Federally funded Research and Development Center" - see https://en.wikipedia.org/wiki/Federally_funded_research_and_development_centers for a good explanation  Note that this term is an official one.
   * "foundation" - self-explanatory
   * "independent_scholar" = If someone authors a paper on his or her own (i.e., not on behalf of any company), then the org type is "independent_scholar."  E.g. "John Smith," retired from NOAA, would be entered into GCIS as name: John Smith; organization: John Smith, with an organization type independent_scholar
   * "intergovernmental" - self-explanatory
   * "International" - self-explanatory but not one that is intergovernmental. Please refer [#459](https://github.com/USGCRP/gcis/issues/459) to categorize international organizations.
   * "municipal" - we don't use this much, but we could conceivably replace "city" with municipal" with a simple database patch
   * "national" - for the equivalent of Federal organizations but for which are outside the US.  Example: "UK Environment Agency" is the British equivalent of our EPA.
   * "ngo" - An official non-governmental organization, such as Greenpeace
   * "non-profit" - A 501c(3) or other non-profit company, e.g. the American Red Cross
   * "private" - somewhat overlaps everything.  The National Academy of Sciences is an example.
   * "Professional society/organization" - self-explanatory.  e.g., the American Psychological Association, the American Geophysical Union
   * regional - e.g. metropolitan planning districts, transit authorities, utility authorities administered by states, interstate councils.  Examples in GCIS include the Western Governor's Association and the South Florida Water Management District.
   * "state" - self explanatory.
   * "State/housed within academic" - examples include various state climatologist offices and state geological agencies which often have a strong affiliation with both the state and university.
   * "territory" - e.g., American Samoa
   * "tribal" - refers to Native American or other indigeneous peoples

### Important Caveats:
   * Very often, an organization can fall into many of these categories.  One can have international research organizations, etc.  Most universities are also non-profit.  In contrast to the US, many universities and companies worldwide are in effect national.  Free to revise the category list as it was developed organically. 
   * GCIS has examples of Canadian provincial organizations, which don't map well into our model.  Suggest adding "provincial" or modifying "state" to read "state or provincial."
   * A revisiting of the organizations that fall into each of these categories (a simple SPARQL query will do it) may be wise to ensure consistency.
   * "Regional" is used on a sub-national scale.  Otherwise such organizations would be "international."
   * This field may be left blank.
   * And finally, if in doubt, check the organization's webpage to see how it defines itself,  Wikipedia is also very helpful.
   * url = the URL of the agency (see At which level do we denote organizations?).  
   * Recall that if the organization name has changed, we leave this field blank.
   * Also begin the URL with "http://" or "http://www.", never with just "www."
   * Don't forget to relate an org with others, if applicable, using the information in the "related organization" box under the "contributors" tab.



###  At which level do we denote organizations? 

A frequently discussed question pertains to the level at which we denote organizations. Examples include the level of university departments, research groups, Federal agencies, line offices therein, laboratories, etc. Although we aren't consistent, we try to maintain the following conventions:
* **Universities:** capture departments and colleges if provided
* **Agencies:** Capture offices, major divisions, and laboratories. Examples: http://data.globalchange.gov/organization/us-environmental-protection-agency-office-air-radiation is one of the main divisions of EPA: http://data.globalchange.gov/organization/national-center-environmental-assessment is an entity within the Office of Air and Radiation.
  * However, we don't go more specific with EPA items.
  * We also include affiliations that authors of papers frequently use in their manuscripts even if they don't seem to follow our specific pattern:
  * For NOAA: http://data.globalchange.gov/organization/earth-system-research-laboratory   
      http://data.globalchange.gov/organization/national-oceanic-atmospheric-administration-national-environmental-satellite-data-information-service  
      http://data.globalchange.gov/organization/noaa-national-climatic-data-center  
  * For the US Forest Service, we stop at the level of the research station, not its underlying field station:http://data.globalchange.gov/organization/us-forest-service-northern-research-station
  * For the USDA Agricultural Research System, we include underlying laboratories
  * Due to various complicated reoganizations that could greatly complicate affiliation tracing, we do not get more specific than NASA flight centers. e.g. http://data.globalchange.gov/organization/goddard-space-flight-center and not any "Goddard Space Flight Center Cryospheric Laboratory."  
* This can get complicated though. An affiliation listed as "US Geological Survey, Menlo Park" should be listed in USGS as "US Geological Survey." However, if the affiliation is listed as "US Geological Survey Menlo Park Science Center," the affiliation should be written as
such and then related accordingly within the USGS hierarchy. This pattern holds for other agencies.
* And finally, we may break this pattern and get more specific in order to match datasets with those in data.gov.  

_**The trick? Remember that we are capturing affiliations, not necessarily employers.**_ This comes into play with entities like the EROS Data Center. Papers with authors having that affiliation do not always list whether the person is a USGS employee. As such, we go by whatever is written.  

A good way to study this is to look at the page for an organization such as the http://data.globalchange.gov/organization/us-environmental-protect
ion-agency and look the nature of the orgs listed.   

Also, note the nature of various related organizations, such as those that are "predecessor of," "division of," etc. When entering an org, one should always check to see if one can relate to other orgs, even if that involves creating an intermediate org.   

**Special exceptions:** We don't go further than "Scripps Institute of Oceanography," Also, per a directive from USGCRP leadership, all entities from the "Climate Change Science Program" (CCSP) must also be attributed to the USGCRP and SGCR. Those attributed to USGCRP should also be attributed to the SGCR but not back to the CCSP.  

Also, if an org is a predecessor of another org:  
* Include both in GCIS
* For the predecessor org, leave the "url" blank
* Relate the two as "predecessor of"

**Note:** an org is considered to be the predecessor of another even if the org's name is the only characteristic that changes (i.e., mission etc.
remain the same).  
**Example:** http://data.globalchange.gov/organization/us-climate-change-science-program  

_**Since we tie people and organizations with publications, we use what is mentioned in the publication**_ even if it has changed. For example, we keep "National Climatic Data Center" even though it is now the "National Centers for Environmental Information." Since it was NCDC at the time of the publication, we keep it as such and employ the methodology used above. As such, if a webpage URL is the same as that in a previous publication but now includes the "National Centers for Environmental Information" banner, we use NCDC in-lieu of NCEI if that is what the author would have seen at the time it was cited.  
One last thing - if an organization relationship changes, do not revise.  Simply update with the new relationship, keeping the older one.

### Examples of orgs that may be called differently in the literature than in how they appear in GCIS.  The following is a non-exhaustive list.
* University of Stockholm is in GCIS as Stockholm University.
* UPMC 6 is in GCIS as Universite de Pierre et Marie Curie
* Cornell University Experiment Station at Geneva, or Geneva Experiment Station is in GCIS as New York State Agricultural Experiment Station
