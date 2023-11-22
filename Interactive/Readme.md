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

HOW WE IMPORTED MULTIPLE OBJECTS

we have multiple objects loaded into the project folder.
this was done by creating new content variables
assigning them to the objects
then calling the content in the needed locations by changing the value of the mosition in the code

HOW WE ANIMATED AND ADDED LIGHTING TO THE MODELS

we added code in the source.cpp where we set the values and positioning to go up and down and looped it.
this made our island model to go up and down to show a floating animation.
we also added values to adjust the speed of the movement as well

to add the lighting we wrote code in the source.cpp file and applied it on the models.
we also gave shine value to change the intensity of the light and adjust when needed.

HOW WE INTERACTED WITH THE MODEL FOR THE VIDEO

We edited the code so that we can interact with the model in the window after running.
W key makes it zoom in
Skey  makes it zoom out
To move up, down, right, left we use the direction keys
