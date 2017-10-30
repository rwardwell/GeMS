This directory contains an ArcGIS toolbox and associated scripts 
for creating, manipulating, and validating GeMS-style geologic 
map databases. See the Docs folder for more information. 

For more information on the GeMS database schema, see
http://ngmdb.usgs.gov/Info/standards/GeMS/


To install this toolbox, either

1) unzip (if necessary) and place the folder GeMS_Toolbox in
a locale of your choice.  Start ArcCatalog or ArcMap, open 
the Arc Toolbox window, right click on empty space in the Arc 
Toolbox window, and select "Add Toolbox".  Then navigate to 
the GeMSv2_Toolbox folder and select file GeMSToolsArc105.tbx 
(if you are running ArcGIS 10.5) or file GeMSToolsArc10.tbx (if 
you are running an older version of ArcGIS).

Right-click again on empty space in the Arc Toolbox window and
select "Save settings" and then "Default" to have the GeMS
toolbox available next time you open ArcCatalog or ArcMap.

or, 

2) place the CONTENTS of the GeMS_Toolbox folder within 
C:\Documents and Settings\<user>\AppData\Roaming\ESRI\Desktop10.5\ArcToolbox\My Toolboxes
(this is the pathname for ArcGIS 10.5 on Windows 7; it may differ with 
other operating systems). Then, in ArcCatalog, scroll to the bottom of 
the left-hand "Catalog Tree" pane, open Toolboxes/My Toolboxes, and the new 
toolboxes should be present. You may need to refresh the listing. 


See the help that is part of the individual tool interfaces for documentation. 
Also the Docs subdirectory of this package for documentation in 
.doc and .pdf format. 

----

Credit

Evan Thoms (USGS) made significant contributions to earlier versions of this
script library. This version is the work of Ralph Haugerud. 

----

Licensing

We wrote these scripts in the course of our employent by the USGS.
To the best of our knowledge, this means they are not subject to U.S. 
copyright. Use them as you will. Where it is appropriate, we would appreciate 
it if you would give credit to the U.S. Geological Survey. 

Module docxModified.py is largely copyrighted by others; see the file header 
for further information. 

----

Known issues with these scripts include:

* "Project Map Data to Cross Section" doesn't always produce the correct 
apparent dip direction. The dip magnitude is correct, but it may be in the
wrong direction.

* "MapOutline" stumbles over some choices of datum.

* ".docx to DMU" and "DMU to .docx" require the lxml Python module, which 
some find difficult to install. The other scripts run without lxml. 

* "Purge Metadata" requires that the USGS EGIS tools for ArcGIS be installed. 

----

Ralph Haugerud
rhaugerud@usgs.gov

10 September 2017