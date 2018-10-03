# GYAZ Handplane Baker Bridge
Blender to Handplane Baker

Blenderartists thread: https://blenderartists.org/t/addon-gyaz-handplane-baker-bridge/1102777

VERSION #11 (Oct 3, 2018)

Baking high poly to low poly geometry in Blender produces inferior results because it has no antialiasing whatsoever. This can be helped to some extent by baking to higher than final resolution but it makes bake times go very high. The solution is to use Handplane Baker which can do 16x supersampling on large textures very fast and is just so much faster than Blender in general. It can organize objects into projection groups and bake all the maps you need at once. This addon makes the process convenient, letting you configure everything from inside Blender and export with a single click.

GYAZ Handplane Bridge:
https://github.com/helluvamesh/GYAZ-Handplane-Bridge

Handplane:
http://www.handplane3d.com/

Get Handplane on Gumroad for free:
https://gumroad.com/l/znpF#

Setup:
1. Download&Install Handplane
2. Install GYAZ Handplane Bridge Addon for Blender
3. Set up handplane.exe path in Addon Preference in Blender

Addon Location:
Properties Window &gt; Render &gt; Handplane Bridge

Usage:
1. Set up projection groups
2. Choose maps to bake
3. Choose destination

way 1:

4. Hit 'BAKE WITH HANDPLANE'
5. Once it's done, the file explorer should popup at export folder/textures

way 2:

4. Hit 'GO TO HANDPLANE'
5. Now Handplane should automatically start and the file explorer should popup, too
6. Drag the .HPB file (which should be selected in your file browser) into Handplane
7. In Handplane go to Output menu and hit BAKE
8. Once it's done, your textures should be in the export folder/textures

Using Tangent Space Normalmaps baked by Handplane in Blender:
To get a normalmap that Blender can use, choose the Unity 5.3 Preset. If you choose Unreal Engine 4 Preset, you can still use the normalmap in Blender by flipping the green channel of the texture in your material.

Extras:
- Save presets for different scenarios
- Checking for common errors:
         -- if lowpoly objects have a uvmap
         -- if lowpoly and cage objects are triangulated
         -- if 'Suppress Triangulation Warning' is True:  if lowpoly and cage objects have ngons
