# KiCAD libraries

KiCAD libraries for OHIS specific components and artwork.  Things like:

* RJ-45 schematic library with all the pins labeled with thier OHIS signals.
* PCB artwork of the OHIS logo, in three different sizes.

# Installation

## Download/Clone git repo

Move to where you keep your git repos, code bases, downloads... where ever you want to store this stuff.  But remember this path, we'll need it below.  For the purposes of installing, I'll call it `[download directory]`.

Download options:

1. ```git clone git@github.com:open-headset-interconnect-standard/OHIS-KiCAD-libraries.git```  
   Good if you want to keep getting updates as they come out.
1. ```wget -o OHIS-KiCAD-libraries.zip https://github.com/open-headset-interconnect-standard/OHIS-KiCAD-libraries/archive/refs/heads/main.zip && unzip OHIS-KiCAD-libraries.zip```  
   Good if you just want a simple "give it to me now" solution that doesn't involve installing `git` if you don't already have it.

(These are Linux commands; If you're on Windows or Mac, you can probably figure out your own instructions.  If you do, please submit a Pull Request to improve this document.  Thanks! -Mark)

## Adding libraries to KiCAD

Start KiCAD, on the main KiCAD page, with the icons on the right side.

### Schematic Symbols

* Go to Preferences -> Manage Symbol Libraries...
* Click the `+` icon at the bottom of the list of libraries.
  * Nickname: `OHIS` (or whatever you want to call it.)
  * Library Path: `[download directory]/OHIS.kicad_sym`
* Click `OK`

### Board Footprints

* Go to Preferences -> Manage Footprint Libraries...
* Click the `+` icon at the bottom of the list of libraries.
  * Nickname: `OHIS` (or whatever you want to call it.)
  * Library Path: `[download directory]/OHIS.pretty`
* Click `OK`

