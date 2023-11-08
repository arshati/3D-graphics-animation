# 3D Graphics and Animation Coursework (Part 2)

## Exporting from Blender
Before exporting the island we disabled the camera and selected all the objects using command A . File -> Export -> .fbx file ->
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

I first created a new blueprint class for the floating island and I made sure it's an actor. When I double-clicked on the blueprint class for the island the blueprint file popped up. In the file, i created a new timeline and added the time frames and disabled the axis not needed. 
i created an event graph where i added this timeline along with a few other functions and reversed and looped it so that the island has a continuous flow of moving up and down to create a floating effect.

## Work done by Prasitha
### Ship and 3 clouds
#### Reference
##### https://www.youtube.com/watch?v=r8ltW7pAN6M&t=256s
##### https://www.youtube.com/watch?v=I7vg-WXBtXY
#### How the animation was done

I first created a new blueprint class for the ship and made it an actor. When I double-clicked on the blueprint class for the ship the blueprint file popped up. In the file, i created a event graph where one of the timeline is the same as the island so that it floats with the island. 
I added new instructions in the blueprint class as well where it makes the shipe move in a circular path around the island according to the spline line i drew accross the screen which was enabled using the construction graph inside the blueprint file.

I made 3 blueprint classes for the 3 clouds and added an event graph with a timeline where i disabled different axis for the different clouds and reversed and looped it. This ensured that the clouds were floating side by side above the island to give a hovering animation effect.

## Work done by Lakshmi 
### 3 Coins and treasure chest
#### Reference
##### https://www.youtube.com/watch?v=1f4B67lpI1k&t=89s
#### How the animation was done

I initially created a new blueprint class for a coin and ensured it was set as an actor. Upon double-clicking the coin's blueprint class, the blueprint file opened. 
Within this file, i included a "Rotation Movement" for all the three coins seperately on different axis and then saved the changes after compiling. This blueprint ensured that the coins are rotating above the treasure chest.

I made the treasure chest float up and down with the island by merging the treaure chest with the coins inside using the merge actors option under the tools section and then imported this actor into the the floating island blueprint class so that the event graph functions applied on the island worked for the treasure chest and coins inside as well. 

### Sequencing
To start the sequencing we added a level sequencer and created a new camera. 
In the camera we added the tranform option and started the sequencing by adding key first then move around in the scence then add the next key at the new time frame to stop.
Similarly we did this throughout the video in parts to show various parts of the scene with all the animation blueprints enabled.
