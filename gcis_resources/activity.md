# Activity Conventions

## Appropriate Use Case:

Activities should be created to connect components of USGCRP reports to the source publication it was created from, in order to convey the process of creating the asset.

i.e.  
- Image back to its dataset  
- Array back to its dataset  
- Figure back to its Article  

We do not create them for non-USGCRP products.

## Field Conventions:
| Field | Description |
|-------|------------- | 
|**identifier**|  The format of the activity identifier going forward should follow the template: "`report_identifier`-`UUID`-`activity`". We may go back and update non-compliant activities, but it is not a priority.|
|**methodology**| The process of creating the resulting object from the input, in the author’s own words and in such a way that another expert partycould reproduce the output.|
|**visualization_methodology**|  The process of creating the visual portion of the output object, if any and if distinguished from the main methodology.|
|**methodology_citation**|  The citation to the methodology, if it has been published.|
|**methodology_contact**|  The point of contact for the methodology, if any.|
|**activity_duration**|  [Valid Interval Formats](https://www.postgresql.org/docs/9.6/static/datatype-datetime.html#DATATYPE-INTERVAL-INPUT-EXAMPLES). Captures the time taken in the process to get from the source object to the final one.|
|**source_access_date** | The date the parent resource was accessed.|
|**source_modifications**|A written description of modifications done to the source object.|
|**modified_source_location**|  The location of the modified source, if available.|
|**interim_artifacts**|  Deprecated outside of NCO assessment activities. The names of files created along the way to create the final product.|
|**output_artifacts** | Deprecated outside of NCO assessment activities. The final output filenames from the process.
|**computing_environment** | Operating systems and versions used to perform this activity.|
|**software** | Primary software (with version) used.|
|**visualization_software**  |Primary visualization software (with version) used.|
|**start_time**  |Time bounds used to restrict the input object. Optional, depending on applicability. If equal to end_time, indicates a temporal moment.|
|**end_time**  |Time bounds used to restrict the input object. Optional, depending on applicability. If equal to start_time, indicates a temporal moment.|
|**dataset_variables**  |A list of Dataset Variables applied in this activity.|
|**spatial_extent**  |Spatial bounds used to restrict the input object. GeoJSON. Optional, depending on applicability.|
|**data_usage**  |**DEPRECATED**.  A description of the way in which input data were used for this activity.|
|**notes** |**DEPRECATED**.  Other information about this activity which might be useful for traceability or reproducability.|
|**duration**  |**DEPRECATED**.  Use activity_duration to document the time taken to perform the activity.


## Provenance Conventions: 
None


## Relationship Conventions:

Associated with two other publications (one parent, one child) as the process of going from one to the other.
