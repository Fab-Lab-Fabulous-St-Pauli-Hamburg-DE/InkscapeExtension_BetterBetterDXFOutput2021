# Inkscape Extension BetterBetterDXFOutput (b2_dxf) 2021
DXF Exporter for Inkscape (Better Better DXF Output Version2021)

Updated version of BetterBetterDXFOutput for recent Inkscape versions. Tested with [Inkscape](https://inkscape.org) version 1.1

## Usage
Copy the three files to your inkscape extension folder.

Linux:
~/.config/inkscape/extensions/ 
On MacOS:
/Applications/Inkscape.app/Contents/Resources/share/inkscape/extensions/

You will see a new filetype (Better Better DXF Output 2021) in the "Save As"/"Save a copy" dialog.

You need to ungroup everything and convert all objects to paths. The extension omits shapes (circles, rectangles, etc). 

CNC Machines use DXF points (not circles) as coordinates for drilling. If a layername ends with drill then all path on these layer(s) will automatically be converted to points. Works best with small circles or rectangles.


## Credits

A big thank you for earlier versions an contributions goes out to

Aaron Spike, Alvin Penner, Bob Cook , Tim Gipson, Jean-Francois Barraud, Chris Madsen, Andreas, Linda Moehsmer, Jamie Tremaine

## more information

For details refer to https://www.fablab-hamburg.org/better-better-dxf-output-2021/
