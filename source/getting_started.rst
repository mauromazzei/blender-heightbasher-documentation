.. highlight:: sh

Getting Started
========================================

1) Setup the Scene
If you're working on a brand new project it's important to set some paramenter in order to make HeightBasher works correctly

1.1) In the "Color Management" Panel switch the "View Transform" from "Filmic" to "Standard"
1.2) In the "Output" Panel set the "Color Depth" to 16-bit or higher
1.3) Set the camera visualization to Z so you will simulate a 2d environment

2) Canvas View


3) Kitstamp View


4) Canvas
The first step is to create a canvas where all the brushes will be drawn, this operation will enable all the other operators.

Now you will have to load as many brushes as you want by clickon on "Add Brush". 
This operation will create an empty object in the center of the canvas, all the empties will be stored in a dedicated Collection in order to keep an ordered workspace.

Each brush is invisible unless you attach a texture to it, you can do it by loading a new texture from the disk or selecting a preloaded texture from the library

Play with the brushes, position, rotation and scale as normals blender object but you can mix all togheter by the Factor slider, it's range is from -1 to 1 and it will merge the mix of the brushes in order to add, mix or cut elements

When you're ready with the canvas you can choose to render it to a file as a texture (it will open a browser dialog) or to render directly to the kitstamp mesh

5) Kitstamp
It's a 3d live-rendered object from the canvas (or from a loaded texture).
You can operate on the rendring with some provided operator:


Subdivision Level:

Displacement Strenght:

Displacement Clamp:

Remesher:

Calculate Smart UV:




