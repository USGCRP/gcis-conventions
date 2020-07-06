# Image Conventions

## Appropriate Image Use Case

Images should only exist underneath Figures.
All Figures should have at least one Image.

For reports done in conjunction with the TSU, the Images should be imported alongside their Figures, or filled in where needed following the pattern they use.

For reports not done with TSU, we may create Images.

Images for Figures with just one panel should be the full Figure (i.e. the same as the image file attached on the Figure record). Images for Figures with multiple panels should be reconstructed from their Figure to contain all relevant information (i.e. labels, legend, etc) rather than simply cropped. If no other option, cropped is better than nothing.

## Field Conventions

| Field | Description |
|-------|------------- |
|**identifier**| Standard UUID identifier.|
|**position**| This is more of a nice-to-have. Not a focus for filling in.Indicator Images do not have Titles.|
|**title**|     Usually imported directly from TSU.Indicator Images do not have Titles.Images should incorporate the Title of their Figure in their Title, plus a relevant distinctive postfix.|
|**description**|   Imported from TSU, if one exists.We do not attempt to fill this in otherwise.|
|**attributes**|    Imported from TSU, if any exists.  For Indicators, filled in if provided.Otherwise, not filled in.|
|**time_start**|  Existing definition fine.  Should match the activity that created it, if any.Blank is okay if irrelevant.If dates aren't exactly specified, they are assumed the earliest possible (i.e. 2017 is 2017-01-01, June 2017 is 2017-06-01). Same for time.|
|**time_end**|      Existing definition fine.  Should match the activity that created it, if any.Blank is okay if irrelevant.If dates aren't exactly specified, they are assumed the latest possible (i.e. 2017 is 2017-12-31, June 2017 is 2017-06-30). Same for time.|
|**lat_max**|       Existing definition fine.  Should correlate with the activity that created it, if any.Blank is okay if irrelevant.|
|**lat_min**|       Existing definition fine.  Should correlate with the activity that created it, if any.Blank is okay if irrelevant.|
|**lon_max**|       Existing definition fine.  Should correlate with the activity that created it, if any.Blank is okay if irrelevant.|
|**lon_min**|       Existing definition fine.  Should correlate with the activity that created it, if any.Blank is okay if irrelevant.|
|**usage_limits**|  Existing definition fine.  Should come from the source of the Figure.  Be certain before filling in; this should be the limits on usage for a public user, not the limits on USGCRP's use of the image.|
|**submission_dt**| Currently, we think this is the last update before submission.*Followup needed.*|
|**create_dt**|     Currently, we think this is the initial creation in TSU's system.*Follow-up needed.*|
|**url**|           Not used.|

## Provenance Conventions

**cito:cites**  

Generally the Figure object will be the thing using cito:cites.  
It is plausible to have a good use case for an image to use cito:cites.

**prov:wasDerivedFrom**

Image is preferred to be the child to `wasDerivedFrom` as opposed to the Figure.  
Many types of publication can be the parent type.  

## Relationship Conventions

**Figure**

- Generally, Figures and Image tend to be one-to-one.  
- It is acceptable if two Figures use the same component images, they may use the same Image object.

**gcmd_keyword**

Not yet implemented, but probably better applied to Figures.

**region**

Not yet implemented.

**file**

Should have a file with the type best suited to its image type. High quality images strongly preferred.

## Unresolved Conventions

### Datetime Values

`submission_dt` and `create_dt` are unclear for initial purpose, current use, and desired use.  
Final determination to be made after conversation with TSU.
