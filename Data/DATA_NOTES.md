# Processing to Produce Working Versions of data
*  'Working Data.xls' is just a copy of "draft_Combined_data_20190917.xls" as
   assembled by Stantec.

*  'Marine Sediment Screening Values simplified.xlsx' is a version of the
   screening values, with unrelated screening levels removed and screening 
   levels for all parameters combined into one table. Simplification done by
   Curtis C. Bohlen, October 7, 2019.

*  'PORTLAND VB TARGET LOCATIONS EDITED.csv' derived from 'PORTLAND VB TARGET
   LOCATIONS.csv' by adding a header row.

*  TARGET LOCATIONS.csv'  Calculated 'decimal degrees (in excel) based on the 
   lat and long values in that file.

*  'Locations Table from Bulk Chemistry Report.docx' Converted by hand by
   copying data from the draft bulk chemistry report, table 2.

*  'Locations Table from Bulk Chemistry Report.xlsx' by copying and pasting from 
   the word document. 
   
*  'Locations Crosswalk.xlsx' derived by hand from that excel file. The
   the "Refined Crosswalk" tab includes the mean locations of the two core 
   samples collected at each sampling location.

# Metadata for the Screening Values included in the Excel files.
The list of PCB congeners and alternate terminology from here:
(https://www.epa.gov/pcbs/table-polychlorinated-biphenyl-pcb-congeners). The table
was copied and pasted into Word from a PDF available at that web site. This
table was used to cross-correlate nomenclature, although as we ended up only
reporting Total PCBs, nomenclature does not matter all that much. 

# GIS Files
'Portland_Dredge_Locations_Screening_Levels_2.mxd' Contains an ArcGIS map file.

The shapefile 'Portland Toxics Location_1' is derived from the lat-long data 
found in 'Locations Crosswalk.xlsx', specifically, the "Refined Crosswalk"
tab in that file. The data was converted following the usual methods for 
converting tabular point location data to GIS data in ArcGIS.  We converted
numerical data to map data using "Display XY Data" and then exported the data 
as a shapefile.
