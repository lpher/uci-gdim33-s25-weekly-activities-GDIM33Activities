# GDIM 33 In-Class Activities
## W1
### Activity 1
[Google Drawing Link.](https://docs.google.com/drawings/d/1S_GXqI5qnxfUtHNd6f6uu1LvPWAfg39THbF85-pkJeA/edit?usp=sharing)

1. Fighting is a genre that is repeated as well as the special effects they come with. They have intense and colorful scenes making the images look busy and fast paced. They exaggerate the effects, making them look more interesting. Bright and vibrant colors are a common trend making things pop more.

2. My tablemate’s style and interest is similar to mine in that we both used bright and vibrant colors. Other than that we have vastly different ideas for games we’re going to make.

3. My LA was Angel. He likes to play Soulsborne games, Minecraft, and Fortnite, all games I enjoy playing too.

### Activity 2
![03bdfc53-8a6c-4e1b-833b-233a806c11ed](https://github.com/user-attachments/assets/8d5f0f73-d1f1-4413-b90c-636ff65fc6ae)

## W2
No assigned devlog this week.

## W3
### Activity 1
<img width="2426" height="3089" alt="8716e53e-f9ae-47ba-99a1-ec7107c2baf3" src="https://github.com/user-attachments/assets/133c5932-feab-4528-9e50-8355f3066c54" />

### Activity 2
1. Saving the event name to a scene variable allows access to this variable from any graph in the scene. Like a singleton, I only need to define it once, which is more efficient than defining the variable multiple times for each graph. Having the event name as a scene variable cuts on the time and effort needed, while retaining function. Doing this is also more advantageous because the event name becomes data making it a lot easier to change and update than if it were hard coded. I would only need to update the original to update all references rather than updating each and every reference. 

2. Using a Debug.Log() node in explore to dialogue transition helped me check whether or not I had set the graph up correctly. Should I have set it up correctly, the clickNpcEventName event would fire and output a log in the console saying “Transitioned ExploreToDialogue.” This would tell me that clicking on the walrus and that the transition from the explore state to the dialogue state triggered by the clicking worked. Otherwise, no message in the console would be logged, which would tell me that I did not set up the transition correctly.

3. It depends on if I can add a lock-on system so that the player can better target the enemy. If I can, then the Set Cursor Lock State would be relevant, but if I can’t, then it wouldn’t be. With the lock-on system, the camera, controlled by the cursor, would be locked on the enemy so that you are always facing them. It is similar to the cursor being locked when you enter the dialogue state when interacting with the walrus, but because the player in my game will still be able to move, the lock-on system will need some sort of tracking system to track the enemy as well as the cursor lock. Having this system will also make player attacks more accurate, which is a nice thing to have but potentially not necessary.

4. I don’t think a game state, or at least the switching between game states, will be relevant to my vertical slice. My vision of the game only includes a fighting state. What I mean by this is that the player will spawn in and fight the enemy until one of them dies. I’m more focused on the fighting aspect for this vertical slice rather than the story, so I don’t think I’ll be adding any exchanging dialogue that requires a dialogue game state.

## W4
### Activity 1
Playable: The player can move with WASD across x and z-axes. They can also move diagonally too. The player can jog with WASD and sprint with SHIFT. Additionally, the player can perform a dodge roll with SPACE.

Playtesting Goals: Testing the dodge roll
- Is the dodge roll responsive? Does it trigger when I press the space bar?
- Is it too responsive or not responsive enough? Does it trigger when I accidentally hit the space bar while trying to sprint?

Playtest Team Members:
- Sebastion
- Rebecca Feng
- Frances Kim
- Kaleb Reyes
- Jess

Playtest Notes:
- Fix idle to sprint transition
- Camera too low at hip, should be at shoulders
- Dodge roll too slow/heavy, should be faster and more fluid
- Edit keyframes to make faster
- Add cursor lock
- Fix burst of speed when transitioning from jog/sprint to dodge
- Fix diagonal dodge
- Fix being able to move while dodging

### Activity 2
1. Yes, a designer could add more dialogue without writing code because we incorporated dialogue into scriptable objects before hand.

2. There isn't a set limit of dialogue nodes the writer could create without code, however, the screen can only show so many options, so eventually the dialogue options will, while being present, won't actually show up on your screen unless you change the scale of UI elemnets.

3. The "Regenerate Nodes" button updates the Node Library so members can be used as nodes.

## W5
### Activity 1
- Basic Steps:
	1. Make Enemy move towards Player using NavMesh.
	2. Make Enemy transition between Moving and Attacking at certain distances from Player.

- Detailed Steps:
	1. Install AI Navigation package. Under GameObject, click AI → NavMesh Surface. This creates a NavMesh Surface GameObject. In its Inspector, click Bake. You should see the ground be highlighted in a light blue.
	2. Create your Enemy GameObject and add a NavMesh Agent Component to it. Create a Movement Script/Graph and make it move the Enemy towards the Player’s position using its NavMesh Agent. Ensure the “Agent Type” field in both the NavMesh Agent and NavMesh Surface are the same for the Enemy. The Enemy should now track and follow the Player wherever they go.
	3. Create a Raycast for Enemy to check distance from Player. In Scene, when clicking on the Enemy GameObject, the Raycast should appear.
	4. Create a State Machine Graph for Enemy with Moving and Attacking states.
	5. Configure the transitions so that they are triggered by whether the Enemy’s Raycast hits the Player. Test with debug logs.
	6. Make Enemy stop moving in its Attacking State (when Raycast hits Player) and resume moving in its Moving State (when Raycast no longer hits Player). Test this in the Scene.

### Activity 2
I created a simple Enemy GameObject and added a NavMeshAgent component to it. I then created a NavMesh Surface in the scene and baked it. After that, I added a Script Machine Component to the Enemy and created a new movement graph that makes  it move towards the player using its NavMeshAgent. I set the target to GameObjects with the "Player" tag" for the NavMeshAgent. When I play the scene, the enemy successfully moves towards the player using the NavMesh.

## W6
### Activity 1
1. I have not been able to implement anything new since milestone 1 because of other projects I have been working on.
2. For now I will link my milestone 1 itch build since that is what I will have people playtest today. Note: I did turn in milestone 1 in late. [Link.](https://lpher.itch.io/gdim-33-verticle-slice-milestone-1)
3. My playtesting goals are:
    - To test feel of newly added attacks and how it flows between movement and rolling
	- To test feel of camera and how it follows the player
	- To test feel of rolling and how it flows between movement and attacking
	- I changed a lot of these values based off of the previous playtesting feedback, so I want to see if the changes I made improved the feel of the game
4. Playtesting notes:
    - Roll and sprinting feel better than first playtest
	- Should be able to move slightly or slower when attacking, not be locked in place
	- Add some sort of lock on
	- Exit transitions should be faster
	- Camera sense too high

### Activity 2
1. I assume the Multiply blend option makes color darker and less saturated because it multiplies mainly decimal values togethor that result in a smaller decimal value which are synomumous with darker and less saturated colors.
2. Multiplying two Alphas would also probably result in a more transparent color because its value is also based off the 0.0-1.0 value range, so multiplying two Alphas with decimal values less than 1 will result in a lower value which is equal to something less transparent.
3. Unity gets UV values from the texture.
4. It sounds interesting to manipulate colors with math.

## W7
### Activity 1
1. The data for the Vertex Color node came from the Shiba’s mesh.
2. The Shiba is blended to obtain the specific colors it now has. There are three main vertices, each associated with their own color being red, blue, and green. They are arranged in a triangle where values in between the three points can give different mixes of colors resulting in new colors other than the main three. This is what the Shiba does in order to obtain its blend of specific colors.
3. The Shiba colored with vertex color appears less detailed than the Shiba rendered with a texture because vertex colors use data from the mesh, which includes the number of vertices and triangles a mesh has. Depending on the number of vertices the vertex color can use, the colored mesh may appear less or more detailed. Since textures don’t rely on the mesh’s vertex data, they are not limited by vertex count.
   
   Vertex color could be useful for low poly games not meant to look good but to run well.
4. There is a patch on the left hind leg that is not the color it should be.
5. I can imagine testing any of the other data under the vertices list in the Shiba’s model like the tangent, position, or UV.
6. That error on the back could be because the shiba’s normal vectors in that one spot are pointing away from itself.
7. Additive sounds like we’re adding something, but I’m not sure what. From what I observed when setting the Blend Mode to Additive, the graph clears all of the darker black spots on the texture. I’m guessing it has something to do with the value of the color black.

## W8
### Activity 1
1. New Features:
   - New attack system architecture
   - Rolling animations have events that turn off and on a separate collider for invincibility frames
   - Attack animations have events turning on and off a separate collider
   - Attacks have damage values
   - Enemy has a health value
   - Enemy health has a UI
   - Damage dealt and accumulated on enemy is tracked and displayed on the UI
   - Implemented toggleable lock on system with a second virtual cinemachine camera that looks at the enemy
   - If locked on and is attacking, player and their attacks will be directed straight towards enemy automatically

2. [Itch Link](https://lpher.itch.io/gdim-33-vertical-slice-playtest-3)

3. Playtesting Goals:
   - Get feedback on new features

4. Playtesting Notes:
   - Player freezes sometimes when spamming attacks
   - Rolling into the enemy repeatedly translates the player upwards
   - When locked on, make camera follow player faster
   - Player can phase through enemy when performing first attack

### Activity 2C
1. Full Screen Pass. It displays the effect across the whole screen.
2. The screen looks like it has the material on but with a lowered transparency when the Lerp is set to 0.5. At zero, the material is completely transparent. At 1, the material is fully untransparent.
3. The Lerp is taking the image projected by the Sample Buffer and the Sample Texture and blending them based on the different float values. A float value zero is basically the Sample Buffer by itself and a float value of 1 would be the Sample Texture by itself. Any float value in between 0 and 1 would project a corresponding image in between the two images.
4. Lerp uses (sin(time)+1)/2 because Lerp can only properly take values from 0 to 1, which are positive numbers, but sin(time) goes into the negatives. Using (sin(time)+1)/2 moves the values all into the positives allowing Lerp to properly use them.
