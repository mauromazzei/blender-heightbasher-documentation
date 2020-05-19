# Getting Started

We provided two additional blender project, nome_file.blend contains an optimized scene and workflow.
Check the instruction at the end of the page

Next, will be explained how to start from a new .blend file.

---

## Setup the Scene
When working on a brand new project it's important to set some paramenter in order to make HeightBasher works correctly

1. In the "Color Management" Panel switch the "View Transform" from "Filmic" to "Standard"
![Color Management Panel]
(https://github.com/mauromazzei/blender-heightbasher-documentation/docs/assets/color_management_panel.png)

1. In the "Output" Panel set the "Color Depth" to 16-bit or higher
![Output Panel]
(https://github.com/mauromazzei/blender-heightbasher-documentation/docs/assets/output_panel.png)

1. Set the camera visualization to Z so you will simulate a 2d environment

---

## Working with Canvas

The first step is to create a canvas where all the brushes will be drawn, this operation will enable all the other operators.

Now you will have to load as many brushes as you want by clickon on "Add Brush". 
This operation will create an empty object in the center of the canvas, all the empties will be stored in a dedicated Collection in order to keep an ordered workspace.

Each brush is invisible unless you attach a texture to it, you can do it by loading a new texture from the disk or selecting a preloaded texture from the library

![HeightBasher]
(https://github.com/mauromazzei/blender-heightbasher-documentation/docs/assets/HB_01.gif)

Play with the brushes, position, rotation and scale as normals blender object

![HeightBasher]
(https://github.com/mauromazzei/blender-heightbasher-documentation/docs/assets/HB_02.gif)

but you can mix all togheter by the Factor slider, it's range is from -1 to 1 and it will merge the mix of the brushes in order to add, mix or cut elements

![HeightBasher]
(https://github.com/mauromazzei/blender-heightbasher-documentation/docs/assets/HB_03.gif)

Each brush can be selected by it's empty object both in the scene or UI


When you're ready with the canvas you can choose to render it to a file as a texture (it will open a browser dialog) or to render directly to the kitstamp mesh

---
## Working with Kitstamp

It's a 3d live-rendered object from the canvas (or from a loaded texture).
You can operate on the rendering with these provided operator:


- **Subdivision Level:**  
Sets the previsualization quality of the output
There are 4 levels.
Level 1 and 2 are fast and gives you the opportunity to check your work during the process.
Level 3 and 4 are more intense and needs time to process, we suggest to use it at the end of the workflow for the final renders


- **Displacement Strength:**  
Sets the extrusion level

- **Displacement Clamp:**  
Helps you to keep the scene clean

- **Remesher:**  
Sets the decimation value of the mesh. We also provided the opportunity of automatically calculate the smart uv


---
## Provided Template

Open the addon zip file, extract `nomefile.blend` and open it
We provided this template with 3 areas

- Canvas view: 2d visualization of the brushes
- HeightBasher UI: Panel that permits you to create/destroy/update canvas, brushes, kitstamp and final rendering
- Kitstamp View: live render of your project

![HeightBasher]
(https://github.com/mauromazzei/blender-heightbasher-documentation/docs/assets/template.png)