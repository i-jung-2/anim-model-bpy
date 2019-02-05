# anim-model-bpy
Export your animated models from Blender in an easy to understand .obj-like format.

### What is this?

This is a simple plugin for [Blender3D](https://www.blender.org/). This exporter allows you to save animated models in a text based, easy to parse format (similar to the Wavefront Obj format).

### Why?

I created this plugin to export some animations I did (and to play them back later in my engine). The format is very simple and it does its job well for simpler animations like walkcycles.
This was used:
 * for the Horse's animation [here](https://youtu.be/t7eaOtnp6Dk?t=90),
 * for the creatures' walkcycle [here](https://www.youtube.com/watch?v=P0UiNxuLM1s).

### Installation

Just copy the folder called *io_export_animmodel* into blender's *scripts/addons* or *scripts/addons_contrib* folder. 

### Usage

In the File->Export menu there should appear an *AnimModel format (.amf)* entry, click on that to export your animation.

### Compatibility & Notes

Tested and works under Blender 2.7 and 2.8. 
Compatible with:
 * Keyframe animation,
 * Modifiers which are not altering the model's triangle count in function of time.
For instance: will not work with fluid simulation for instance, but it will work with armature or ocean modifier.

### What's next?

 * Add a file format specification,
 * Create repositories for the Java and C++ importers, link them here.