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

Make sure that the Units of the SVG document are set to "mm" and the x any scaling is set to 1 (File-> Document Settings->Page Tab / Datei -> Dokumenteneinstellungen -> Seite). If you open a SVG file that was created with an older Inkscape version the scaling might be set to something else than 1.

### Drilling ###

CNC Machines use DXF points (not circles) as coordinates for drilling. If a layername ends with drill then all path on these layer(s) will automatically be converted to points. Works best with small circles or rectangles.


## Credits

A big thank You for earlier versions and contributions goes out to

Aaron Spike, Alvin Penner, Bob Cook , Tim Gipson, Simon Arthur, Jean-Francois Barraud, Chris Madsen, Andreas, Linda Moehsmer, Jamie Tremaine

## More information

For details refer to https://www.fablab-hamburg.org/better-better-dxf-output-2021/ and the [repository wiki](https://github.com/Fab-Lab-Fabulous-St-Pauli-Hamburg-DE/InkscapeExtension_BetterBetterDXFOutput2021/wiki)
