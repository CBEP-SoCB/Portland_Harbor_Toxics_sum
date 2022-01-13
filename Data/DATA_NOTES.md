# Processing to Produce Working Versions of data

## Toxics Data
### `working_data.xls`
A complex Excel file, with 6 tabs.  Each tab contains data for one or more 
groups of contaminants :

Tab              |  Contents 
-----------------|------------------------------------------------------
'Combined'       | Typical EDD format combined raw data, by sample, with CAS numbers, units, QA/QC Flags, etc.
'Metals'         | Data on metals, summarized by Site (Values are averages of usually two cores)
'PAHs'           | Data on PAHs,  summarized by Site
'PCBs'           | Data on PCBs, summarized by Site
'Pesticides'     | Data on Pesticides, summarized by Site
'Grain Size_TOC' | Data on metals, summarized by Site

For the most part, we pulled data from the "Combined" tab, and selected the data 
we wanted for each group by matching names of the parameters on each of the
other tabs. Tabs are fairly well described in the worksheet, so we do not 
provide additional metadata here.

## Screening Values
### `Marine Sediment Screening Values simplified.xlsx`
Contains sediment screening values, principally from NOAA's SQuiRT Tables, with 
unrelated screening levels removed and screening levels combined into one table. 
A second tab contains relevant metadata.

While this table includes some screening values scaled to organic-matter 
weighted concentrations, we did not use them in this report because of limited
availability for the totals we chose to emphasize.

## Location Information 
### `Locations Crosswalk.xlsx` 
Was derived from data on the location of individual vibracore samples, and
information on which samples were assigned to each location. The the "Refined
Crosswalk" tab includes the mean locations of the two core samples collected at
each sampling location.

The file contains multiple tabs.  "Raw Crosswalk" provides details on the
relationship between vibracore locations ("VB##"), and Sample Location ('CSP##'
and 'CSS##') numbers, along with descriptive names of the sample locations. 
"Historical Uses" is a copy of Table 1 from the Campbell Scientific Report. It
contains information on historical uses of the harbor near  sampling locations 
that may affect what type of contaminants are founds nearby. 
"VB Locations"" contains spatial information (in DMS format, WGS 1984) for the
vibracore locations.  "Refined Crosswalk" combines data from the other tabs for 
GIS.

Contents of the "Refined Crosswalk" Tab have the following meanings:

Column     | Contents                        
-----------|-----------------------------------------------------------------
Location   | Name of sampling location
SAMPLE_ID  | Sample Location (CSP## or CSS#) ID
VB_ID      | ID numbers for the related vibracore locations.
avglatDD   | Average latitude, in decimal degrees (WGS 1984) of related vibracore locations
avglongDD  | Average longitude, in decimal degrees (WGS 1984) of related vibracore locations
Avg_Sample | Average of the sample depths of the two vibracores (feet)
Dredge_max | Anticipated maximum dredge depth (feet)
Sources    | Historical uses of the adjacent pier or source area (From Table 1).# GIS Files

### GIS Data
The shapefile 'Midpoint_Core_Locations' is derived from lat-long data shared
by Campbell Scientific and Stantec.  The attributes are based principally
on Table 2 of the Campbell Scientific Report.  Historical uses of  the area an 
potential sources are from Table 1. 

Attribute  | Contents                        
-----------|-----------------------------------------------------------------
FID        | Arbitrary identifier added by ArcGIS
Location   | Name of sampling location
SAMPLE_ID  | Sample Location ID
avglatDD   | Average latitude, in decimal degrees (WGS 1984) of related vibracore locations
avglongDD  | Average longitude, in decimal degrees (WGS 1984) of related vibracore locations
Avg_Sample | Average of the sample depths of the two vibracores (feet)
Dredge_max | Anticipated maximum dredge depth (feet)
Sources    | Historical uses of the adjacent pier or area (From Table 1).

