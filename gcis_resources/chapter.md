# Chapter Conventions

## Appropriate Chapter Use Case

Chapters are created for USGCRP Products and for external report that are being cited in GCIS a large number of times at a chapter specificity. See the CSSR and the IPCC reports, respectively.

## Field Conventions

| Field | Description |
|-------|------------- | 
|**report_identifier**|The GCIS identifier of the report this resource belongs to. | 
|**title**| Official published chapter title. Does not include a subtitle, unless needed for uniqueness. Doesn't include "Chapter 1:" prefix. Doesn't include the Report name. See CSSR as exemplar of good title convention.|  
|**identifier**|Title of the chapter with dashes in place of the spaces.|
|**number**| The official published chapter ID, if any. (i.e. 1, 2, 3, A, B, C, i, ii, etc). Likely blank for chapters like front matter and executive summary.  Does **not** determine chapter ordering. See *sort key*.|
|**url**|The direct URL for the given chapter.  Same as what the chapter DOI, if any, would resolve to. Blank if chapter does not have its own URL. Do not use the report URL. | 
|**sort key**| The internal number to make the chapters sort in order.|
|**doi**| the DOI for the Chapter, if any. Blank if not. Do not use the report DOI. | 

## Provenance Conventions

- Chapters use `cito:CitedBy` and `cito:Cites`.  
- Chapters should be created with their internal citations as `cito:Cites`  
- We are generally only concerned with `cito:CitedBy` when it is citations by a future USGCRP product. We do not try to proactively find external citations.  

## Relationship Conventions

**report**
   - must exist.

**figures**/**findings**/**tables**

   - only populate these for USGCRP reports
   - if an external federal agency is creating a report and collects metadata in GCIS-compliant processes, they may populate those records.
     - See good convention exemplar `epa-multi-model-framework-for-quantitative-sectoral-impacts-analysis-2017`

**Contributors**

 - only populated for the USGCRP produced reports.
 - For some reports, we list all authors on the report and not per-chapter. (See CSSR) 
 - Generally speaking, follow how the report links authors. 
   - If they are listed on the report as a whole, list on the report. 
   - If they have the authors specified by chapter, list on the chapter.

**Files**

   - should be the downloadable PDF of the chapter, usually hosted externally to GCIS. 
   - Populated for USGCRP produced reports. 
   - Maybe populated for external reports.


**gcmd_keywords**
 - not to be used for the moment. To be determined.
 
**regions**
 - not to be used.

## Unresolved Conventions

### Published Stand-alone Chapters
   
   - What to do for report chapters that are also available as separately published reports (i.e. CSSR ch Executive Summary & The CSSR Executive Summary PDF), **that also specify distinct citations**?
       - should we have both publications (chapter version & report version) in gcis?
       - should both have a DOI, and should they be distinct?
       - Discussion Issue [#19](https://github.com/USGCRP/gcis-conventions/issues/19)
