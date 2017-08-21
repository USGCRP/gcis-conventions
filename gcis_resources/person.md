# Person Conventions

## Identifier Convention

[See default: Number](./Defaults.md#Number)

Created automatically.

## Adding People to GCIS
  - `id`
    + Leave as is, as this is an internal identifier used by GCIS.
  - `first_name`
    + Examples: Jeffrey; C. Ben; Richard A.
    + Basically, we use the first initial and middle name, the first name, or the first name and middle initial
    + Note that some authors publish under variations of the same name depending on the publication.  In that case, we use the following system:
    + If an NCA3 authors, use what is used there
    + else: if Health Assessment author, use what is there
    + else: the most complete formal name used in a GCIS publication
    + Note that we only keep one name in GCIS (i.e., no aliases).  For example, "Robert E. Wolfe" and "Robert Wolfe" cannot both exist in the database and be affiliated with the same article if they refer to the same person.  This too can be changed.
  - `middle_name`
    + currently does not show on html, hence we use the middle name or middle initial in the "`first_name`" field (UPDATE upon completion of https://github.com/USGCRP/gcis/issues/298)
  - `last_name`
    + The person's last-name, including if it's hyphenated
    + Note that sometimes first and last names may be flipped in publications (common with many non-US author
  - `orcid`
    + The person's ORCiD (see http://orcid.org)
    + If not information is available on the person's ORCiD page to definitvely attribute something to that person, leave the field blank.  This situation occurs very commonly when people do not leave identifying information on their ORCiD pages.  Hence, it is possible that someone else with the same name created that ORCiD.
    + Very often, people will just link their ORCiDs to their ResearcherID pages, which many times is enough to make a definite match with the article author.
    + Enter only the sixteen digit value with hyphens, with nothing else.  Also, refrain from adding other IDs like Scopus since the system will return an error if the value exceeds sixteen digits and doesn't begin with the standard "0000."
  - `url`
    + An "official" URL for that person
    + It could be a page on one's company website.
    + It could provide any sort of information, and can even be an obituary.
    + Could also be a wordpress account if that could be identified as an official page (i.e., created by the author).
    + Could also be accounts on gulfbase.org
    + Note: many add their lab's URL in their ORCiDs.  Normally, we go with the page on the lab's server about the person, not the main page for the lab, but either way works
    + Avoid linking to third-party pages, such as a UN or other entitty's writeup of that person in order to advertise his or her upcoming speech - this occurs quite often.
    + It is advisable to use the most up to date website if possible.  e.g. if someone has a website on one university's server from his/her graduate school days and one from a subsequent research appointment, use that from the research appointment.
    + Think of it this way: if I wanted to advertise my official website next to my e-mail address on a business card, what would I use beside social media websites, researchgate, academia.edu, and linkedin?
    + Update if necessary but don't go out of one's way to locate all not working URLs.

