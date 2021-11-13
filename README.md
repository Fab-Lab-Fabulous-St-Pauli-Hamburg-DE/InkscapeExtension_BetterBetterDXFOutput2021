# Inkscape Extension BetterBetterDXFOutput (b2_dxf) 2021
DXF Exporter for Inkscape (Better Better DXF Output Version2021)

Updated version of BetterBetterDXFOutput for recent Inkscape versions. Tested with [Inkscape](https://inkscape.org) version 1.1

## Installation ##

Copy the following four files to your inkscape extensions folder. 

**b2_dxf_outlines.py** (Main program file)

**b2r_dxf_outlines.inx** (Extension description. This file makes the extension known to inkscape)

**dxf_templates_b2.py** (A DXF Template. It is used to generate the DXF output.)

**simpletransform.py** (This file contains several functions to make handling of transform
attribute easier. Probably all/many of them are nowadays available anyway in inkscape.)

Linux:
~/.config/inkscape/extensions/ 

MacOS:
/Applications/Inkscape.app/Contents/Resources/share/inkscape/extensions/

## Usage ##
You will see a new filetype (Better Better DXF Output 2021) in the "Save As"/"Save a copy" dialog. Maybe a restart of inkscape is necessary.

You need to ungroup everything and convert all objects to paths. The extension omits shapes (circles, rectangles, etc). 

All colors are omitted / converted to black. If you need colors please have a look at bigbluesaw's old version of the extension (the link is in the [wiki](https://github.com/Fab-Lab-Fabulous-St-Pauli-Hamburg-DE/InkscapeExtension_BetterBetterDXFOutput2021/wiki) of this project). It seams not difficult to add but obviously needs testing. We welcome a pull request.

If you open a SVG file that was created with an older Inkscape version and the scaling in the DFX is wrong please save a copy of the SVG (using "Save as") delete anything in the file. Create a 100x100mm rectangle. Convert the rectangle to a path save the file again and send us the file. Old inkscape SVG versions seam to use a different scaling factor.

### Drilling ###

CNC Machines use DXF points (not circles) as coordinates for drilling. If a layername ends with *drill* then all path on these layer(s) will automatically be converted to points. Works best with small circles or rectangles.


## Credits

A big thank You for earlier versions and contributions goes out to

Aaron Spike, Alvin Penner, Bob Cook , Tim Gipson, Simon Arthur, Jean-Francois Barraud, Chris Madsen, Andreas, Linda Moehsmer, Jamie Tremaine

## More information

For details refer to https://www.fablab-hamburg.org/better-better-dxf-output-2021/ and the [repository wiki](https://github.com/Fab-Lab-Fabulous-St-Pauli-Hamburg-DE/InkscapeExtension_BetterBetterDXFOutput2021/wiki)
