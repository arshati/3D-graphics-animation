HOW WE LOADED THE 3D MODEL

To load the 3d model from blender we had to do the following:

Before exporting:
Merged all the objects and fixed any nodes issues that were there.
open layout mode
open uv editor and add a texture with a name
changed the width and height to 2048
in layout mode you add image textrures
copy the image texture and paste for all the materials in layout mode
edit mode in 3d viewport
data properties and add a uv map
select object in edit mode, unwrap & wrap it to get all the textures and materials properly

for baking the model:
scene
render
cycle
bake type diffuse

after baking:
we duplicate the object
remove all the old materials and add the texture of the original
then save it

while exporting:
file
export
gltf seperate
saved the png images to the textures folder
include -> selected objects
data and mesh -> apply modifiers, UV's, models and vertex colors
export into the opengl folder
call it in the source cpp file

HOW WE ANIMATED THE MODEL

HOW WE INTERACTED WITH THE MODEL FOR THE VIDEO

We edited the code so that we can interact with the model in the window after running.
W key makes it zoom in
Skey  makes it zoom out
To move up, down, right, left we use the direction keys
