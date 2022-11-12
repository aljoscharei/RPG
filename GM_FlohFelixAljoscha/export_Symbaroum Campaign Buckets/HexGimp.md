- https://sites.google.com/view/ddhorizons/cartography/hexgimp
	- HexGimp was created by Isomage. I've updated hexGimp's script to be compatible with GIMP 2.10.18, and added in layer grouping to make map creation easier.

To install hexGimp onto your machine do the following:

-   Go to [](https://www.google.com/url?q=https%3A%2F%2Fwww.gimp.org%2F&sa=D&sntz=1&usg=AOvVaw3QwFCpGejGPFtVdIlhI6W7) [https://www.gimp.org/](https://www.google.com/url?q=https%3A%2F%2Fwww.gimp.org%2F&sa=D&sntz=1&usg=AOvVaw3QwFCpGejGPFtVdIlhI6W7) and install GIMP 2.10.18
    
-   Copy hexGimp-0.0.5.1 onto your script directory. Normally the path is: C:\Program Files\GIMP 2\share\gimp\2.0\scripts
    
-   Copyone of the hex.*.zip files into your brushes directory. The * refers to the version of the hex you would like to use for your map. Normally the path is: C:\Program Files\GIMP 2\share\gimp\2.0\brushes .
    

To create a hex map go File, then New Hex Map v6. It will present various options. Once you click OK it will render your hex map. If you encounter errors it's usually because the script cannot find the blank hex file under brushes.

When using creating your own hexmap via hexGimp you'll want to Snap to the grid so the hexes will align properly. To do this go to View -> Snap to Grid.

  

In the files below there are three hex compilations.

-   Hex.v1.zip is pretty close to BECMI's standard color hexes.
    
-   Hex.BB.1.zip is the current set I'm working with where I've started to recolor some hexes and custom hexes or overlays for 2020.
    
-   Hex.DJS.2.7z is the updated set for 2021 I am tweaking colors and hexes to better create a better visual.
    
-   Hex.CRPG.1.zip is for hex conversions from old games in the 80's and 90s.
    

Note: For historical purposes hexGimp-0.0.5.zip is the original file created by Isomage. It does not always run correctly with the current version of Gimp.
- [[HexGimp.zip]]

  

[](https://sites.google.com/view/ddhorizons/cartography/hexgimp/overlay)


-  https://sites.google.com/view/ddhorizons/cartography/hexgimp/tutorial-existing-bitmap-to-hexgimp
	- [[D&D Horizons - Tutorial - Existing Bitmap to hexGimp.html]]!


[https://forum.rpg.net/index.php?threads/hex-maps-talk-to-me-of-putting-hexes-on-real-world-maps.691138/post-16844821](https://forum.rpg.net/index.php?threads/hex-maps-talk-to-me-of-putting-hexes-on-real-world-maps.691138/post-16844821)

  

  

Briefly (Gimp 2.8):

  

Open your map image in Gimp (be sure it's in RGB mode Image/Mode/RGB).

Figure out how big you want your hexes in pixels.

Create a new layer above your map layer.

Set FG color to white, BG color to black (or some other visible color for your hex lines).

Go to Filters/Distorts/Mosaic

Pick Hexagon.

Set tile size to your hex size.

Set tile height to 1.

Set tile spacing to the width of lines you want in pixels.

Set tile neatness to 1 (for exact hex tiles).

Set color variation to 0.

Check the FG/BG lighting box.

Uncheck Antialiasing, Color averaging, Allow tile splitting, Pitted surfaces.

Hit OK.

  

Von meinem iPhone gesendet