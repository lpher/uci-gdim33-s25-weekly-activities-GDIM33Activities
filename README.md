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
