<!-- Markdown Docs: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax -->
## Name: Abiodun Odufuye
### Module: Dev Log 7
<!-- Repeat the below as needed-->
### Date: [03/30/2026]

#### Goals for this Module
<!-- Example Template (include the brackets to make a checklist, fill them in as appropriate
- [ To acquire more knowledge throughout my creation of the project I'm working on ] Goal 1
- [ To finishing designing the hexagonal tilemap in Unity ] Goal 2
- [ To eventually implement player logic ] Goal 3
-->

#### Progress
- **What I accomplished**:
  - Summarize completed tasks or progress made.
    - I scoured through Youtube to gain knowledge from Unity videos regarding how hexagonal tile maps work and a way to implement them into my project. I managed to a fully functioning pointy topped hexagon with 3 different tile types (Bronze, Silver, Gold) my game will utilize. I've also started on the player logic portion by first creating images of my player tokens and rendering them as prefabs.
- **Challenges faced**:
  - Describe blockers, bugs, or issues encountered.
    -  The grid generation pertaining to my hexagonal tile map was not cooperating with my game scene to the point of starting the game scene would not load up the tile map at all.
- **Solutions**:
  - Detail how you addressed challenges or your thought process.
    -  The tile map code I got from one of the Youtube vide I watch was too outdated for Unity 6 to handle so I instead went for the simple Manhattan distance diamond pattern. Dictionary key checking was added also in place to ensure the existence of tile coordinates. 

#### Learnings
- Key insights, techniques, or concepts explored.
  -  Manhattan method is beyond superb to use when dealing with tilemaps as it calculates the distance between two points to achieve a desired endpoint. Its very useful for emulating not only 4 directional movement but for diagonal direction as well

#### Free Thinking
- Brainstorm or reflect on design ideas, architecture patterns, or potential improvements.
  -  I wonder why certain function like FindObjectOfType() is considered too oudated to use via Unity 6 and pushes you to use newer terminology 
  - I wonder why SortingLayer is seen as a crucial element in developing games and will cause certain objects to disappear from the game scene entirely
<!--

- Example prompts:
  - "What if the player interactions were asynchronous instead of real-time?"
  - "How could ECS improve performance in this system?"
  - "Does my current design support scalability? How can it improve?"
  
-->

#### Next Steps
- Tasks or experiments to focus on during the next session.
  -  I'll working on having my player tokens interact in the game world, a dice mechanic for player movement, and soon create the item types for my players to use in their journey around the map