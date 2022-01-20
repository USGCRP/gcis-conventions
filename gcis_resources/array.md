# Array Conventions
## Appropriate Use Case

- Holds the low level content of a Table entity.  
- Tables may contain multiple arrays.
- If a table has multiple arrays, the table caption should briefly explain how the arrays relate.  
- Tables should note the units in the caption.
- Arrays are created whenever a table is created.
- Header Values may be cleaned up for proper importing into GCIS.  
- Data values should not be changed. If they are for any reason, it should be noted in the Table caption.  
- If the provided raw data has seemingly extraneous data (i.e. totals not displayed in the published work), we reserve judgement on including them on a case by case basis. 
- All data published in the final published Table or Graphic should be included.  
- We try not to upload CSVs to create arrays, but instead paste in well formatted data.
- If the provided raw data is not in a CSV format, we reserve judgement on formatting them on a case by case basis.

## Field Conventions

| Field | Description |
|-------|------------- | 
|**identifier**|  Automatically created UUIDs.  In the case of multiple arrays per table, we may identifier the array with short, internally distinct identifiers the show which is which.  See the arrays under the [Sea Surface Temp Indicator 2018 Table](https://data-stage.globalchange.gov/report/indicator-sea-surface-temperature-2018/table/indicator-sea-surface-temperature-2018)|
|**rows_in_header**|  Usually one, indicates how many rows to be ignored as headers, non-data.|
|**rows** | The actual data, including headers, if any, stored as a database array. Avoid special characters, if possible.|

## Provenance Conventions

**prov:wasDerivedFrom**

With very rare exceptions, should be used on the Array instead of the Tables.  
Most commonly, Arrays are connected to a Dataset via an Activity.

**cito:cites**

Generally the Table object will be the thing using cito:cites.
It is plausible to have a good use case for an array to use cito:cites.

## Relationships

`table`  
Arrays should always belong to a Table. The relationship is generally added through the Table object. Multiple arrays are added in their original order.



