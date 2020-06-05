# Interface

Heightbasher UI is a composite of two panels: **Canvas** and **Kitstamp**.

![Heightbasher UI](img/interface1.png)

---
## Canvas Panel

In this Panel we can create and manage the brushes that will create the final output

![Heightbasher Canvas Panel](img/interface2.png)

- **Create Canvas**  
creates the base canvas, it should be the first operator to launch otherwise will be impossible to create brushes

- **Add Single Brush**  
create a new brush as an empty object in the scene. moreover creates an item in the brush list with these properties:  
-- Load and assign a texture from disk  
-- Select texture from library  
-- Duplicate brush  
-- Remove brush  
-- Set it's factor. The range is -2, 2. Negative factor will force Heightbasher to work in a subtractive way

>Each brush can be selected from the library or the brush list, double click on the brush list to rename it to a more convenient name

![Heightbasher Interface Brushes](img/interface6.png)

- **Render to file**  
Render the canvas to a texture and save it to disk for future use.

- **Render to kitstamp**
This operator creates a new kitstamp object (and destroys a previous one if it exists) and renders the canvas to it.
It is useful because permits you to edit the canvas 2d height map and render on the fly to the 3d kitstamp without leaving blender or saving to disk and then reload a texture


---
## Kistamp Panel

In this panel we can create and control the 3d version of the canvas output and sets the rendering parameters

![Heightbasher Kitstamp Panel](img/interface3.png)

- **Create Kitstamp**  
Creates the kitstamp object that will render the canvas heightmap in a 3d environment

- **Kistamp Texture**  
You can choose to load a texture from the disk or from the blender library

- **Subdivision Level**  
Sets the previsualization quality of the output
There are 4 levels.
Level 1 and 2 are fast and gives you the opportunity to check your work during the process.
Level 3 and 4 are more intense and needs time to process, we suggest to use it at the end of the workflow for the final renders

![Heightbasher Kitstamp Panel](img/interface4.png)

- **Displacement Strength**  
Sets the extrusion level

- **Displacement Clamp:**  
Helps you to keep the scene clean

![Heightbasher Kitstamp Panel](img/interface5.png)

- **Remesher:**  
Sets the decimation value of the mesh. We also provided the opportunity of automatically calculate the smart uv