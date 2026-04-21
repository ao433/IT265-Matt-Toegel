<!-- Markdown Docs: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax -->
## Name: 
### Module:

<!-- Repeat the below as needed-->
### Date: [04/20/2026]

#### Goals for this Module

- [ To finish the Store button functionality during a player's turn  ] Goal 1
- [ To get started on the Use button functionality during a player's turn  ] Goal 2
- [ To provide functionality to item types (Pickaxes, Lamp, TNTs, and Helmets)] Goal 3


#### Progress
- **What I accomplished**:
  - Summarize completed tasks or progress made.
    - Since my last dev log, I've created a plethora of gaming systems for my project furthering it to a state of playability: player tokens can now be spawned onto the tile map, dice mechanic for player movement is fully functionable, a number of tiles are highlighted based on the dice roll number a player received, deck system now prints out a card on player's turn, and a Do Nothing that allows for a player to end their turn after a dice roll.
- **Challenges faced**:
  - Describe blockers, bugs, or issues encountered.
    -  Player tokens disappearing off the tile map once the game scene loaded up, UI objects not being ratio'd correctly resulting in those elements becoming too big or small depending on the project window size, tile highlight not showing up in the game scene at all, mouse clicking not registering the Do Nothing button, and dice mechanic being too loose that rolling again wouldn't transfer to the next player's turn thus becoming broken
- **Solutions**:
  - Detail how you addressed challenges or your thought process.
    -  Player tokens and tile highlights disappearing was the working of improper layer sorting so I had to manually get that in order in the Inspector window, had to set the Xs and Ys on the UI objects to 0 so their anchors could be located in the bottom left of the screen causing less disortion when project screen is a different size, fixed the coroutine for the dice roll to properly end after rollDuration, and prompted the Do Nothing button onto the M keybind as the raycast on the mouse wouldn't register on that button at all

#### Learnings
- Key insights, techniques, or concepts explored.
    -  Debug logs have been an impeccable habit I've been implementing in my code whenever I get stuck as the error message can notify exactly when goes wrong in the code and cuts down on the potential time wasted when you're left in the dark tackling bugs in your code

#### Free Thinking
- Brainstorm or reflect on design ideas, architecture patterns, or potential improvements.
    -  I wonder what's the use of private variables in game code when even the engine you're working on won't recognize that instance of code?
    - Would it be worth if my player tokens have distinctive health in a game that has various item types for the players to interact with the environment or towards other players?
<!--

- Example prompts:
  - "What if the player interactions were asynchronous instead of real-time?"
  - "How could ECS improve performance in this system?"
  - "Does my current design support scalability? How can it improve?"
  
-->

#### Next Steps
- Tasks or experiments to focus on during the next session.
    -  I plan to finish up my entire Use/Store/DoNothing system so my players will have the ability to commit to drastic choices throughout traversing the ever-perilous the game world