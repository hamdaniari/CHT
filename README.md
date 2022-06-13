# CHT
Tutorial of Conjugate Heat Transfer in OpenFOAM

This tutorial is based on the tutorial from wiki
https://openfoamwiki.net/index.php/Getting_started_with_chtMultiRegionSimpleFoam_-_planeWall2D

The modifications are:
1. The mesh size in the solid region is larger than the orginal file
2. The mesh was made by using ANSYS (SpaceClaim for modelling and ANSYS mesh for meshing)
3. The interface between solid and fluid is named manually in ANSYS meshing (by name selection)
4. Solid region and fluid region is not shared in topology 
5. Thus, interface in solid is named "solid_to_fluid" and fluid interface is named "fluid_to_solid"

Due to the mesh was not made using blockMesh, we need rename the BCs. Please take a look in "run" file

How to run
type on your terminal (ignored $)
$./run
