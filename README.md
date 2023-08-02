# Shyblowers-OrcaSlicer-Profiles
This is the beginning of my collection of printing profiles for the [OrcaSlicer][87cdc829] slicing software for FDM printers.

You might use it according to the license included in this repository. Non-commercial means in this context, that you must not sell the profiles themselves or derivatives of them, without my permission, but you may of course use them for commercial printing.

Profiles will added and improved to the extent that my time allows.

## Directory structure and naming conventions
I'm trying to keep the hierarchy as flat as possible and therefore made it only 3 levels deep:
- **printer**  
  - printer profiles for different nozzle diameters
  - **type of filament**
    - processing profiles for different layer heights
    - **filaments**
      - filament profiles

The attributes I have not organized hierarchically are directly coded into the filenames so you have to combine printer, processing and filament profiles according to this nomenclature, and only use a filament profile which is e.g. made for 0.2mm layerheight with the appropriate processing profile made for the same layer height.

Filament profiles are named according to this scheme:  
_\<brand and type\> \<color\> @\<printer\> \<nozzle diameter\> x \<layer height\>.json_

I also tune each color of the same brand and type of filament separately because even the color pigment often affects the behavior of the filament and you might at least need a different Pressure Advance value, which is particularly important with white.

This structure may be subject to change.

## Notes
These profiles have been created for the 1.6.3 release of [OrcaSlicer][87cdc829] using my Bambu Lab X1C with original Bambu Lab Hot Ends and are supposed to be used with the proper processing and printer profiles which can be found upwards in directory hierarchy. When used in a different manner the chances that they will work for you as they do for me might be greatly reduced.  

They might also work with the recent Bambu Studio 1.7.0 beta where most of OrcaSlicers advancements seem to be included, but I've not tried it yet.  

**YOU MUST DISABLE FLOW AUTOCALIBRATION WHEN USING THESE PROFILES, OTHERWISE MY CAREFULLY, MANUALLY CONFIGURED FLOW AND PRESSURE ADVANCE VALUES WILL BE OVERRIDDEN WHICH MAY MOST PROBABLY LEAD TO UNEXPECTED RESULTS**

  [87cdc829]: https://github.com/SoftFever/OrcaSlicer "OrcaSlicer by SoftFever"

As advised by Bambu Lab, flexible filament like TPU must not be used from within the AMS. All my flexible profiles have been created by using the spool holder on the back of the machine, feeding it into the printer through a Y splitter.

## NO WARRANTY; DISCLAIMER
I MAKE NO WARRANTY OF ANY KIND, WHETHER EXPRESS, IMPLIED, STATUTORY OR OTHERWISE, INCLUDING WITHOUT LIMITATION, MERCHANTABILITY, FITNESS FOR A PARTICULAR USE AND NON-INFRINGEMENT. YOU ASSUME ALL RISK FOR YOUR USE OF THE CONTENT OF THIS REPOSITORY, INCLUDING WITHOUT LIMITATION ANY HARM CAUSED BY VIRUSES, WORKS, OR OTHER DAMAGING MATERIALS. IN NO EVENT DO I GUARANTEE ANY RESULTS FOR YOU. I DO NOT WARRANT THAT ANY PORTION THEREOF, IS ACCURATE, ERROR OR BUG FREE, OR THAT ITS USE WILL NOT NEGATIVELY AFFECT OTHER SOFTWARE OR HARDWARE.
