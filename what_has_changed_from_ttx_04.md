# What has changed from TTX 0.4?

# Cloud
TTX is now a cloud based service. You can review your 3D-Model and its history in the web. There are no more database files.

# Collaborators
In order to collaborate online, TTX-Cloud has user accounts and [permissions](../detailed_documentation.md#permissions) to make sure only the right people have access to your model. Users can have admin, write or only read permissions.

# Staging
TTX is more verbose and transparent about what is going to happen to your model. A staging dialog will popup before any change is applied and will tell you in detail about what is going to happen to which element.

# Filters
To make sure the SAP geometry doesn't screw up Revit's geometry TTX now has filters. Filters let you define what information comes across different platforms Eg. always let SAP update Revit Sections but not the other way round.

# Sections
TTX Now stores section sizes as well, so your online 3D model is as precise as possible. This allows you to review and discuss or even preset the online model easily.

# Revit
New supported elements:
* Openings
* AdaptiveComponents

# Tekla
* TTX now creates one Grid System and then creates individual grid planes inside that Grid System to represent TTX grid lines.
* The unknown material dialog has been removed in anticipation of a more robust TTX material mapping process (coming soon).
* The actual geometry cross-section of beams, braces, and columns, are now being translated to TTX. This allows for custom section interoperability in the future.

# SAP
Custom frame sections created by Section Designer are supported.

The following analysis elements are now supported for interoperability:
* Releases
* Restraint
* Load Pattern
* Load Combination
* Load Case
* Point Load on Frame
* Linear Load on Frame
* Uniform Load on Area (Shells)


# ETABS

Custom frame sections created by Section Designer are supported.

The following analysis elements are now supported for interoperability:
* Releases
* Restraint
* Load Pattern
* Load Combination
* Load Case
* Point Load on Frame
* Linear Load on Frame
* Uniform Load on Area (Shells)

# Grasshopper
New Elements:
* Openings
* Releases
* Restraint
* Load Pattern
* Load Combination
* Load Case
* Point Load on Frame
* Linear Load on Frame
* Uniform Load on Area (Shells)

# RAM
We now have a Ram Client supporting: Beams, Columns, Braces, Walls and Floors.

#Excel
We have an Excel Client allowing you to manipulate parameter values or change sections or materials.