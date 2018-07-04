# adobe-photoshop-resave-images-droplet
AppleScript droplet for batch re-saving different image file formats using Adobe Photoshop into CMYK color space (for print prepress).


## Installation
Follow these steps to create your droplet application:

1. Make sure you have **Adobe Photoshop CC 2018** installed on your Mac.
2. Open `main.scpt`using **Script Editor** (`/Applications/Utilities/Script Editor.app`)
3. Open the script **Library** (Command+Shift+L)
4. Click the '**+**' button and select the **Adobe Photoshop CC 2018** app (`/Applications/Adobe Photoshop CC 2018/Adobe Photoshop CC 2018.app`)
5. Compile the script (Command+K) and make sure there are no error prompts
6. Export as:  
	**File format:** Application	
7. Drag & Drop a batch of [supported] image files on the droplet app

## Scripts
* **main**.scpt

## Script details
###  main
This script batch processes and converts raster images files to the [**CMYK** color mode](https://en.wikipedia.org/wiki/CMYK_color_model) [if possible] ideal for prepress workflows.

**SUPPORTED FILE TYPES:** [TIFF](https://en.wikipedia.org/wiki/TIFF), [PSD](https://en.wikipedia.org/wiki/Adobe_Photoshop#File_format), [Photoshop EPS](https://en.wikipedia.org/wiki/Encapsulated_PostScript), [JPEG](https://en.wikipedia.org/wiki/JPEG).

Any of these file types that supports the CMYK color mode is supported. Files that are in **Grayscale** color mode are left as is as they conform with CMY**K**.  


**UNSUPPORTED FILES:** 

Some file formats that do not support CMYK (like [PNG](https://en.wikipedia.org/wiki/Portable_Network_Graphics), [GIF](https://en.wikipedia.org/wiki/GIF) or [Targa](https://en.wikipedia.org/wiki/Truevision_TGA)) are not converted and marked with a gray Finder tag instead in order for you to review this files manually afterwards.


**UNSUPPORTED COLOR MODES:**

Files that contain [Duotone](https://helpx.adobe.com/photoshop/using/color-modes.html#duotone_mode) or [Multichannel](https://helpx.adobe.com/photoshop/using/color-modes.html#multichannel_mode) color modes are marked with a yellow Finder tag for you to manually review afterwards as these use special color channels.

----------------------
These scripts are distributed under the GNU GPL v3 license.  
See the LICENSE file for details.