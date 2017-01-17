# Known Limitations in Konstru \(beta\)

# Revit

## IDs

Two people using the same Konstru Model in Revit should sync their Revit Models using Worksharing. Otherwise, each model will have a different ID in both local Models, which might cause confusion.

## Elements

Konstru currently supports the following element types: Columns, Braces, Beams, Floors, Walls, Grids, Groups, Levels.

Analytical elements such as loads are not supported at this time.

## Openings

Symbolic lines in openings might be interpreted as the opening outline. To avoid this misinterpretation, either do not use symbolic lines or make sure the symbolic lines have a line-style \(eg. Thin-Lines\) applied. When symbolic lines have a line-style, Konstru will recognize them as annotations.

## Adaptive Components

Adaptive Components will be uploaded and downloaded by Konstru if family and type exist in the Revit file. Adaptive Components  will be displayed on the web as spheres marking their location points.

## Names

Revit does not support special characters in names for Levels or Grids. The following characters are allowed:  
`A-Z a-z 0-9` and `. _-/'()"`. All Element names are written to the `Konstru_Name` Text parameter. It should be created automatically. If the text parameter is not created automatically, you should create it manually.

## Custom Profiles

Revit handles profiles in the following order:  
1. Search for types loaded in the document  
2. Search for standard types on the local drive  
3. Create new family and type

## Characters

To make sure everything is working as expected, limit characters in your type and element names to our list of supported characters:  
`0-9` `A-Z` `a-z` `._-\/()"×<>[]ñÑÄÖÜäöü`

# Excel

Excel can be used only to manipulate parameter values, change sections \(by name\), and change materials \(by name\). Geometries and IDs can not be modified using Excel.

# SAP2000

## Plugin

SAP2000 supports the external plugins. Konstru is developed as plugin and can be reached within SAP2000 models.

## Custom Profiles

Custom sections in regular shapes \(I,C,W,Rectangular etc\) are supported. The irregular shapes are not currently translated via Konstru.

## Grids

Grids are not supported in SAP2000 due to OAPI limitations.

## Levels

There is no model object to represent Konstru levels in SAP. Levels are not supported in SAP.

## Openings

Openings are not supported in SAP.

## Analysis Elements

Thermal Load assignments on joint, frame and area not supported.  
Uniform load to frame \(area loads\), Strain loads, surface pressure, temperature, wind pressure loads are not supported.  
Diaphragms are not supported.

## Beams, Braces and Columns

Beams, Braces, and Columns are created as frame objects in SAP2000. Label \(the unique name\) can be overwritten only if the Konstru name is not duplicated in another frame object.

Directions: There is no special frame direction. Frames can be drawn in any way possible. 

## Floors and Walls

Floors and Walls are created as area objects in SAP. The sloped area objects are currently ignored by Konstru but maintained in the model.

# ETABS

## Plugin

ETABS supports the external plugins. Konstru connects to ETABS as plugin and can be reached within ETABS models.

## Custom Profiles

Custom sections in regular shapes \(I, C, W, Rectangular, etc\) are supported. Custom profiles can be created via Section Designer while Konstru download. The irregular shapes currently are not translated via Konstru.

## Grids

Grids are not supported in ETABS due to OAPI limitations.

## Levels

Konstru Levels are stories in ETABS.

## Analysis Elements

Thermal Load assignments on joint, frame, and area not supported  
Uniform load to frame \(area loads\), Strain loads, surface pressure, temperature, and wind pressure loads are not supported.  
Diaphragms are not supported.

## Updates

Due to OAPI limitations the area's geometry and frame's geometry currently cannot be updated.

## Beam, Column and  Braces

Beams, Braces, and Columns are created as frame objects in ETABS. ETABS automatically labels the frames as B, D, and C depending on the orientation. Vertical frames are columns, horizontal frames are beams, and the all others are braces. Unique Name can be overwritten only if the Konstru name is not duplicated in another frame object.

Directions: ETABS automatically flips the frames \(start and end points\). ETABS flips the frames per end point coordination. The start point is smaller in respective axis but this is only correct when the member the parallel to x, y or z axis. The z axis is the governing axis, for example, when x and y values are negative values. Therefore, the lower z value is the start point. Similarly, if the z value is the same for both ends, the X axis is the governing axis for y values. Therefore, the lower x value is the start point.

## Floor and Walls

Floors and Walls are created as area objects in ETABS. The sloped area objects are currently ignored by Konstru but maintained in the model.

The ETABS API does not support creating properties for area objects. Therefore, Konstru cannot automatically create wall or floor sections in ETABS.

# Tekla

## Installation

Due to the way Tekla loads new tools and how Konstru is deployed, after the initial install, if nothing appears after hitting the Konstru toolbar button, a restart is required. This restart is necessary only once after the initial install.

## Elements

Supported Konstru Elements: Beams, Braces, Columns, Floors, Grids, Levels, Walls.

## Openings

Floor openings are supported, but openings created with shafts from Revit are not. No other openings are supported.

# RAM

## Elements

Supported Konstru Elements: Beams, Braces, Columns, Floors, Grids, Levels, Walls.

## Openings

Floor openings are supported. No other openings are supported.

## Levels

As RAM is very level driven, it is best to have valid levels present. In cases where valid levels are not present, levels will be automatically created at column endpoints. Framing elements falling within plus or minus 3 feet of a certain level will be created on that level.

