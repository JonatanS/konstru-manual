# Desktop Clients

##Limitations for Etabs:
###Levels:
TTX-Cloud Levels are translated to stories in Etabs.

###Grids:
TTX-Cloud currently does not support Grids in Etabs.

###Beams, Braces and Columns
**Conversion:**
Beams, Braces and Columns are created as frame objects in Etabs. Etabs automatically labels frames as B, D or C, depending on their orientation. Vertical frames are columns, horizontal ones are beams, all others are braces.

**Direction: **
ETABS automatically flips frames, depending on their end point coordinates. The start point coordinates are smaller than end point coordinates, if the member is parallel to the x, y or z-axis. The z-axis is the governing axis, when x and y values are negative values (the lower z value is the start point). Similarly, if the Z-value is the same for both points, the X-axis is the governing axis to determine frame orientation. In this case, the point with the lower x-value is the start point.

###Floors and Walls
Floor and Wall objects are created as area objects in Etabs.

###Openings
Openings are created as area objects in Etabs. The "opening" attribute is set to true. Etabs Openings don't have host (parent) objects, and their thickness is 0.

##Limitations for SAP2000:
###Levels:
TTX-Cloud Levels are not supported in SAP2000.

###Grids:
TTX-Cloud currently does not support Grids in SAP2000.

###Beams, Braces and Columns
**Conversion:**
Beams, Braces and Columns are created as frame objects in Etabs. Etabs automatically labels frames as B, D or C, depending on their orientation. Vertical frames are columns, horizontal ones are beams, all others are braces.

###Floors and Walls
Floor and Wall objects are created as area objects in Etabs.

###Openings
Openings are currently not supported in SAP2000