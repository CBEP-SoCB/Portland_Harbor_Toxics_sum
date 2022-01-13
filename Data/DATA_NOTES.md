# Processing to Produce Working Versions of data
*  'Working Data.xls' is a copy of "draft_Combined_data_20190917.xls" as
   assembled by Stantec.


## Screening Values
### `Marine Sediment Screening Values simplified.xlsx`
   Contains sediment screening values, principally from NOAA's SQuiRT Tables,
   with unrelated screening levels removed and screening levels combined into 
   one table. A second tab contains relevant metadaa.
   
   
   
   
*  'Locations Crosswalk.xlsx' derived by hand from that excel file. The
   the "Refined Crosswalk" tab includes the mean locations of the two core 
   samples collected at each sampling location.

# GIS Files
The shapefile 'Midpoint_Core_Locations' is derived from lat-long data shared
by Campbell Scientific and Stantec.  The attributes are based principally
on Table 2 of the Campbell Scientific Report.  

Attribute  | Contents                        
-----------|-----------------------------------------------------------------
FID        | Arbitrary identifier added by ArcGIS
Location   | Name of sampling location
SAMPLE_ID  | SAmple Location ID
avglatDD   | Average latitude, in decimal degrees (WGS 1984) of related vibracore locations
avglongDD  | Average longitude, in decimal degrees (WGS 1984) of related vibracore locations
Avg_Sample | Average of the sample depths of the two vibracores (feet)
Dredge_max | Anticipated maximum dredge depth (feet)
Sources    | Historical uses of the adjacent pier or area (Source has been lost. May be unreliable).

