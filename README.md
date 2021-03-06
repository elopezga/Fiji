# Fiji Distribution for MAPIR Cameras
This repository contains the Fiji distribution for use with MAPIR cameras. The distribution contains various plugins and resources such as luts, flat-fields, and calibration files.

Functionality for MAPIR cameras includes:
- Convert RAW to TIFF
- Correct vignette of RAW and JPG images
- Image index processing
- Calibration

### Installation
Fiji is an all-in-one package that contains everything you need to run the application. We have added plugins to extend the functionality of Fiji for our MAPIR cameras. You may choose to do an easy installation or a custom installation if you already have Fiji but would like to extend its functionality to support our MAPIR cameras.

#### Easy Installation (RECOMMENDED)
For easy installation, download the .zip for your system in the [Packages](/Packages) directory. Everything you need is included within the package that you choose. To launch, simply run the ImageJ executable.

#### Custom Installation
If you already have your version of Fiji, but would like to extend its functionality to support our MAPIR cameras, you may do so by downloading the plugins and its dependencies. Download the [Calibration](/Calibration), [Survey2](/Survey2), [luts](/luts), and [plugins](/plugins) directories and place them at the root of your Fiji installation; this is the directory where the ImageJ-xxx executable resides. The plugins and luts directories should already exist, simply replace these directories with the ones in this repository.

### Using Plugin
Within Fiji's submenu, you will see a MAPIR option. The MAPIR plugin contains 5 tools that aids with post processing.
- Post Process Survey2 Images From Directory: Automatically corrects vignette on RAW and JPG based on Survey2 camera model used. RAW images are converted to TIFF format.
- Image Index Processing From Directory: Creates color and floating point NDVI or DVI images from a directory of images in ImageJ/Fiji that recorded visible light in one band and near-infrared light in another.
- Image Index Processing From Displayed Image: Creates color and floating point NDVI or DVI images from an image displayed in ImageJ/Fiji that recorded visible light in one band and near-infrared light in another.
- Generate Image Calibration Coefficients: Calibrate a digital photograph acquired with a single NIR-modified camera using visible bands and NIR-band-to-reflectance values.
- Apply Calibration Coefficients To Directory: Apply the calibration coefficients calculated from “Generate Image Calibration Coefficients” to a directory of images. The calibrated images are saved as JPEG and/or TIFF.

### Directory
- [Calibration](/Calibration): Contains files for the calibration plugin.
- [Fiji.app](/Fiji.app): Demonstrates example Fiji installation with MAPIR plugin. You can use this copy of Fiji, but please note that it is for a 32-bit Windows system.
- [Packages](/Packages): Contains easy installation deployment for various systems. Downloading a zip packages for your system and extracting is sufficient to start using Fiji.
- [Survey2](/Survey2): Contains plugin dependencies such as flat-fields, exiftools, and macros.
- [luts](/luts): Look up tables
- [plugins](/plugins): Plugins for Fiji. 
