BlenderGcodeImport
==================

Python script to load gcode files produced by Slic3r into Blender

This work was based on the plugin (now defunct?) by Simon Kirkby.  I wrote this because the previous one 
did not work with more recent (2.7.0) versions of Blender.

To use this download the plugin and start Blender

File -> User Preferences 

Find the "Addons" tab and at the bottom click the "Install from File..." button.
Navigate to the python script here, select the file and click "Install from File..." in the upper right corner.
This should show the plugin:

Import and visualize gcode files generated by Slic3r (.gcode)

Click the checkbox to enable the plugin and close the user preferences window.

Now the "File->Import" menu should contain a new entry "Slic3r GCode (.gcode)" which you can use to import
your gcode file.