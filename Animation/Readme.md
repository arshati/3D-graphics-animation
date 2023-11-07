# 3D Graphics and Animation Coursework (Part 2)

## Exporting from Blender

Before exporting the island we disabled the camera and selected all the objects using A. File -> Export -> .fbx file ->
We adjusted the settings, changed the path mode to copy, limit to selected objects, object type to mesh, under geometry - smoothing -> normal to face. We exported this fbx file into the unreal project folder. 

## Importing into Unreal

To import the fbx file in unreal, we first created a project folder in unreal Games, from the content drawer we imported the fbx file into the content. We selected all the materials, objects etc and dragged and dropped it into the unreal screen. 

## Link referred for exporting/importing

##### https://www.youtube.com/watch?v=BBYIw23sFyU

##Issues that arised and their solution

While importing the island, the water's material and textures had disappeared. To resolve this issue we created a new material and changed the color. We added this new asset into the content drawer and applied it on the water in the floating island 3d model. 

During the animation, when we tried to float the island, there were a lot of conflicts due to having multiple objects. To resolve this issue we merged all the actors from the tools in unreal. This ensured that the blueprint for the floating animation applied to the whole island with the merged objects.

All the objects that were made in blender using plane, had an issue while importing into unreal where objects would disappear from different angles. To resolve this issue we increased the thickness using solidify modifier in blender and imported the fbx file for the selected objected again. 

## Workdone by Arshati
### Island
#### Reference
##### https://www.youtube.com/watch?v=r8ltW7pAN6M&t=256s
#### How the animation was done

I first created a new blueprint class for floating island and I made sure it's an actor. When i double clicked on the blueprint class for the island the blueprint file popped up. In the file, we created a new timeline
