# scaleSM Plugin for ImageJ/Fiji
Measuring distances in images obtained with surgical microscopes (SM) with ImageJ/FIJI.
scaleSM is a plugin (https://imagej.net/imagej-wiki-static/Plugins) written in python using ImageJ commands (ImageJ Macro language).  

  1. First you need ImageJ or Fiji installed on your PC. We recommend Fiji, which can be downloaded under https://fiji.sc/ 

  2. Download scaleSM.py from our repository

  3. Two options installing the plugin:

     3.1. Via Plugin Installation
       - Start ImageJ/Fiji
       - Navigate to "Plugins" -> "Install Plugin.."
       - Select scaleSM in the folder you downloaded it to
       - Restart ImageJ/Fiji

     3.2. Moving scaleSM.py to plugin folder
       - You can manually move the scaleSM.py file to the plugin folder of the ImageJ/Fiji app folder
       - Restart ImageJ/Fiji

     After restarting ImageJ/Fiji scaleSM can now be found under "Plugins" usually on the bottom of the drop down menu.

     Troubleshooting: If your having problems launching the plugin. Try installing jython (https://imagej.net/scripting/jython/) via the ImageJ/Fiji Update function or manually.

Using scaleSM to measure objects in images obtained with surgical microscopes (currently available only for Zeiss Kinevo 900).
Images have to be scaled first to allow measurement. The scaleSM plugin facilitates the scaling. Measurement can be performed by various ImageJ/Fiji options (lines, squares, irregular shapes,..). 

Important: To allow scaling the images must be obtained with the Zeiss Kinevo "Position Memory function" (normal "photos" are stored without sufficient metadata). The image folder must contain the pertinent images saved in .png or .jpg format along with their corresponding .xml files otherwise scaling is not possible.

  1. Open ImageJ/Fiji and select scaleSM found in the plugin section
  2. A dialog box should open up
  2.1. Select the surgical microscope used (currently only for Zeiss Kinevo 900)
  2.2. Select the image file format .jpg or .png (necessary since problems occurred with automatic selection)
  2.3. Hit OK
  4. A dialog box should open up asking you to navigate to the image folder you want to scale
  5. After selecting the desired folder, the plugin will scale the images creating duplicate .tif files with the suffix scaled
  6. Now you can use "File" -> "Open.." to open a scaled image and measure distances with the "line tool" (select two point in the image) and hit STRG + M (or "Analyze" -> "Measure")
  7. The scaling in pixel/mm is saved in a .txt file and can also be checked in ImageJ/Fiji under "Analyze" -> "Set Scale..."

Troubleshooting: If your having problems launching the plugin. Try installing jython (https://imagej.net/scripting/jython/) via the ImageJ/Fiji Update function or manually.
