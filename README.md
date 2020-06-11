BlenderGcodeImport
==================

#### ntoff forked from: https://github.com/iraytrace/BlenderGcodeImport
#### damistry forked from:  https://github.com/ntoff/BlenderGcodeImport

__Note:__ There are 2 branches, one is `Master` (the default), the other is `Animated`. The `Master` branch does NOT include the layer animation script, this might be handy if you only want the full model imported and no keyframes set for animating the visibility of the layers, and has the bonus of being faster because it doesn't have to work on each of the layers, setting the visibility and keyframes. The `Animated` branch DOES set the keyframes for each layer to create the timelapse effect of it looking like the print is being built up over time.

#### What is?
A gcode importer script for blender that can automatically animates the layers to create a timelapse effect of building up the model layer by layer.

I (damistry) modified the code to work for Blender 2.8

#### To use
* Download the plugin and start Blender
* Enter the user preferences -> addons -> install addon from file -> choose the downloaded plugin -> enable it -> save user preferences if you'd like it enabled every time blender starts.
* Import gcode using Object -> Import GCode (.gcode)
* Toggle the system console (window - toggle system console) to keep an eye on the import script as blender may appear to have frozen but as long as you still see it processing the frames, just let it be. 
* Once the import is complete, make sure all layers are visible (fast forward to the end of the timeline), highlight all objects with A, and press ALT + C, and choose "mesh from curve" to convert all the imported curve objects into meshes.
* From there on out it's your choice whether you render the entire thing to a cool movie set to dramatic music with CGI explosions, or render to a single frame for artistic style.

#### Additional:
You can usually safely ignore any "unknown command" outputs. The script is just saying "hey, I dunno what this gcode does" and for the most part it won't matter because it's not printing anything so it doesn't need to know how to turn a fan on or how to modify the acceleration values.
