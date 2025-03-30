## Geometry Nodes Tree to Distribute Rooftiles over the faces of a Mesh.

The Blender V4.4 file includes a Geometry Nodes Tree which distributes Rooftiles above the faces of a mesh. The Blender file also includes example Roof objects and example tiles.

When you download the Blender file into your Asset folder, the Nodes Tree and Object become available as Assets in you Asset Browser. 


In the Geometry Nodes Modifier you will have the following options to tailor the Distribution of the Rooftiles:

![image](https://github.com/user-attachments/assets/6df319a0-6975-49ab-a5ef-e937eb078eeb)

**Rooftile object:** The Blender Rooftile object which will be distributed over the roof faces.

**Rotate X, Y and Z:**  Rotate the Rooftile object in it's Local space 

**Rooftile overlap x & y:** The amount of overlap of the Rooftile in the x & y direction

**Height of tiles above roof face:** Distance (height) between the mesh face and the orgin on the Rooftile. If your roof mesh is skewed the Rooftiles may only be partly generated above the mesh faces. This can be solved by increasing this height value.   

**Tiles on Faces/Edges/Vertices?:** The Nodes Tree creates a grid above the face. This grid is used to Instance the Rooftiles above the Roof face. You can select here if you want the Rooftiles instanced on the Faces, Edges or the Vertices. If you have Slates as a Rooftile, you can select Edges as this allows the Slates to alternate half tiles between the vertical rows.

**Scales tiled faces:** This allows you to re-size the generated grid face instanced with Rooftiles as required. 

**Show original Geometry?:** Show the original Geometry.

**Minimum/Maximum slopw in degrees:** Rooftiles will only be generated on faces with a slope between the min/max degrees you define here.

**Show Convex Hull? & Convex Hull Scale:** If you have a simple straight forward roof mesh you may be able to use the Convex Hull to "shave off" (Boolean Intersect) the excess Rooftile. The Convex Hul Scale can be adjusted.

**Execute Boolean Intersect with the Convex Hull:** Here you can activate the Boolean Intersect with the Convex Hull (non-destructive)


The GN Tree uses Raycasting to determine where Rooftiles need to be placed obove the Roof face. The tree is provided as-is and you may use it anyway you like.
