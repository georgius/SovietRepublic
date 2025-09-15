### Overview

Contains source models, materials and workshop items for [Pedestrian tunnel crossings](https://steamcommunity.com/sharedfiles/filedetails/?id=3568764267).

Models are created with [Blender 4.5.3 LTS](https://www.blender.org/download/releases/4-5/ "Blender 4.5.3 LTS").

### Convert Blender file to game file
For converting Blender file to game file is necessary to enable WavefrontOBJ format (Edit -> Preferences -> Addons, search for Wavefront, must be checked).
Steps:
1. **save Blender file**
2.  select all objects (Object Mode -> Select -> All)
3. mirror selected objects by X Global (Object Mode -> Transform -> Mirror -> X Global) - that is why you need to save Blender file
4. export to Wavefront OBJ (File -> Export -> Wavefront (.obj)):
	required Wavefront OBJ options:
	- Write Normals
	- Include UVs
	- Write Materials
5. copy exported .obj file to game workshop folder (somewhere in workshop_wip subfolder of WRSR)
6. run ModelViewer.exe from WRSR install folder
7. import exported .obj file from game workshop folder
8. save as NMF file (same game workshop folder)
9. remove *.bbox and *.fire files (game will recreate these files)