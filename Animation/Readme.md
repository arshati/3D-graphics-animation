# 3D Graphics and Animation Coursework (Part 2)

## Exporting from Blender

Before exporting the island we disabled the camera and selected all the objects using A. File -> Export -> .fbx file ->
We adjusted the settings, changed the path mode to copy, limit to selected objects, object type to mesh, and under geometry - smoothing -> normal to face. We exported this FBX file into the unreal project folder. 

## Importing into Unreal

To import the FBX file in Unreal, we first created a project folder in Unreal Engine, and from the content drawer, we imported the FBX file into the content. We selected all the materials, objects etc and dragged and dropped them into the unreal screen. 

## Link referred for exporting/importing

##### https://www.youtube.com/watch?v=BBYIw23sFyU

## Issues that arise and their solution

While importing the island, the water's material and textures disappeared. To resolve this issue we created a new material and changed the color. We added this new asset to the content drawer and applied it to the water in the floating island 3D model. 

During the animation, when we tried to float the island, there were a lot of conflicts due to having multiple objects. To resolve this issue we merged all the actors from the tools in Unreal. This ensured that the blueprint for the floating animation was applied to the whole island with the merged objects.

All the objects that were made in blender using plane, had an issue while importing into unreal where objects would disappear from different angles. To resolve this issue we increased the thickness using the solidify modifier in the blender and imported the FBX file for the selected object again. 

## Work done by Arshati
### Island
#### Reference
##### https://www.youtube.com/watch?v=r8ltW7pAN6M&t=256s
#### How the animation was done

I first created a new blueprint class for the floating island and I made sure it's an actor. When I double-clicked on the blueprint class for the island the blueprint file popped up. In the file, we created a new timeline

## Work done by Lakshmi 
### Coin
#### Reference
##### https://www.youtube.com/watch?v=1f4B67lpI1k&t=89s
#### How the animation was done
I initially created a new blueprint class for a coin and ensured it was set as an actor. Upon double-clicking the coin's blueprint class, the blueprint file opened. Within the file, we included a "Rotation Movement" and then saved the changes after compiling.
