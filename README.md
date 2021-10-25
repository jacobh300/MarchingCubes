# MarchingCubes
A rendering program based on the Marching Cubes algorithm that allowed for generating a polygon mesh based on a set of 3D values.

Look into the PDF file for a more detailed explanation of the algorithm 

![alt text](https://i.imgur.com/RraAgHg.gif)

Interface/GUI

![alt text](https://i.imgur.com/e8D6wSw.png)


● The Top left sliders will configure how big of a space the algorithm will sample

● The first vertical slider on the right (Cube Resize Icon) will configure the scale of the
cubes generated each sample. Smaller sizes will create a more detailed mesh however
will become highly computationally dependent.

● The second vertical slider (Filter icon) will determine the Iso Level, lower will accept
lower level iso values to be activated, while higher iso level will filter out higher level iso
values of vertices.

● Interpolate will toggle between interpolation of edge points, enabling edge points to
estimate how far along the edge lines they should appear.

● Interpolation cutoff slider, will tell the algorithm how much of a difference the iso level
needs to be in order for the edge point to calculate a different position rather than in the
middle of the 2 vertices.

● Invert button, The invert button will swap the filter from filtering out vertices to filtering in
vertices. This will create a mesh with back faces invisible (due to backface culling) but
also a mesh that's created inside out. You can use this to create a “cave” like mesh, and
allow your first person camera to drop inside to explore depending on how much of the
space you filtered in/out

![alt text](https://i.imgur.com/scIFnPw.gif)
