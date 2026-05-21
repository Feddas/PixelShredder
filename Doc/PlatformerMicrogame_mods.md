Official information on using learn.unity.com/project/2d-platformer-template has been mostly deleted. As described on https://learn.unity.com/g/2d-platformer-creators .

1. List of all mods: https://web.archive.org/web/20230611003114/https://learn.unity.com/project/2d-platformer-template
2. [Modify Tilemap](#modify-tilemap)
3. [Modify Triggers](#modify-triggers)

# Modify Tilemap

2D Platformer Mod: Paint Your Level
- Tutorial, Foundational, 5 Mins
- Summary: Let’s customize our level by painting on the Tilemap!
- Micro-Games: Platformer
- Last updated: April 17, 2023
- Modify Tilemap was copied from [archive.org](https://web.archive.org/web/20230605020247/https://learn.unity.com/tutorial/2d-platformer-challenge-paint-your-level?uv=2019.3&projectId=5c8838feedbc2a0ee1e7e030#5c8932f9edbc2a1410354fda)

## 1.Paint Your Level
Let’s customize your level by painting on the Tilemap! Our level is made of several Tilemaps. We can paint and edit these layers to create levels.

1. Open the Tile Palette Window by going to **Window > 2D > Tile Palette**

2. In the Tile Palette window, hold Alt while clicking and dragging in the palette to scroll around. Zoom in and out of the Tilemap Palette by scrolling the mouse wheel.

3. Find the platforms and the clouds in the Tile Palette by scrolling around the palette.

4. Select the Paintbrush tool in the Tile Palette toolbar.

5. Select “Level” in the Active Tilemap dropdown menu.

6. Click on a block in the Tilemap Palette to select it for painting.

7. Return to the Scene window. Click and drag in the Scene view to start painting the selected block.

8. To erase blocks, select the Eraser tool.

9. With the Eraser tool selected, click on a block in the Scene view to erase it. It will only erase Tiles that are on the currently selected Active Tilemap.

10. Enter Play Mode and test your new level!

## 2.TileMap Extra Credit
Stretch your Unity skills with these additional mini-mods.

- Change up the entire level to your own design. Add enemies, tokens, and more platforms to your custom level. Test your creation with friends!

## 3.TileMap Deeper Learning
Go deeper in your exploration of the techniques used in this mod.

In this mod, you "painted" a level of your 2D Platform game using Unity's Tilemap system. This system was designed to help creators easily build tile-based 2D games and levels. To learn more about these concepts, check out these related Unity tutorials:

- [Live Session: 2D World Building with Tilemap and Cinemachine](https://web.archive.org/web/20230605020247mp_/https://learn.unity.com/tutorial/live-session-2d-world-building-w-tilemap-cinemachine-for-2d) - This recorded live session follows the creation of a 2D game using Tilemap and Unity's Cinemachine system for camera control.
- [Ruby's Adventure: 2D Beginner](https://web.archive.org/web/20230605020247mp_/https://learn.unity.com/project/ruby-s-2d-rpg) - This Learn Project steps you through the complete creation of a 2D RPG game, and features heavy use of the Tilemap component.

# Modify Triggers

2D Platformer Mod: Custom Triggers
- Summary: Triggers are a powerful part of Unity and game development. Learn how to hook-up your own custom trigger to activate a confetti celebration!
- Micro-Games: Platformer
- Last updated: April 17, 2023
- Modify Triggers was copied from [archive.org](https://web.archive.org/web/20230605005307mp_/https://learn.unity.com/tutorial/platformer-mod-custom-triggers?uv=2019.3&projectId=5c8838feedbc2a0ee1e7e030)

## 1.Custom Triggers

1. In the **Menu Bar**, select **GameObject > 2D Object > Sprites > Square**. This will be our “trigger”.

2. In the **Inspector** under the **Sprite Renderer** component, change the **Sprite** field by clicking on the circle next to **Square**. Search “**TileGround**” and double-click on it.

3. Using the **Move** and **Scale** tools, adjust the tile so that it covers up a portion of the scene that the Player can walk over.

4. Rename the **GameObject** to “**ConfettiTrigger**”.

5. In the **Inspector**, click on Add Component and search for **Box Collider 2D**. Click on it to add it.

6. In the **Inspector**, under the **Box Collider** component, check the **Is Trigger** box.

7. In the **Inspector**, click on **Add Component** and search for **Simple Trigger**. Click on it to add it to the ConfettiTrigger.

8. Drag in **Player** from the Hierarchy to the **TriggerBody** field inside of the Simple Trigger script.

9. In the Project View, find **ConfettiCelebration** under **Assets > > ModAssets > Particle Prefabs > ConfettiCelebration**.

10. Drag the **ConfettiCelebration** prefab into the Hierarchy on top of **ConfettiTrigger**. This will make it a child of ConfettiTrigger, and make it centered on top of it.

11. Click on **ConfettiTrigger**, and in the Simple Trigger component click **+** underneath On **Trigger Enter ()**.

12. From the **Hierarchy** (not the Project View!), drag in **ConfettiCelebration** onto the **None (Object)** field. Alternatively, you can click on the circle next to **None (Object)** to search for it.

13. Click on the dropdown that says **No Function** and select **ParticleSystem > Play**.

14. Now we just need to hide the **ConfettiTrigger** mesh so that you don’t see it on the road. Uncheck the box next to **Sprite Renderer**.

15. Click Play and watch the confetti fly out when you cross the box!

## 2.Triggers Extra Credit
Stretch your Unity skills with these additional mini-mods.

- Add more **Confetti Triggers** around the track.
- Have multiple **Confetti Celebrations** activate on one trigger.
- Use different effects for the triggers - see the **Platformer Mod: Bouncy Sparkly!** for different effects you can use.
- Triggers are very powerful - you can make all sorts of cool stuff happen! Can you figure out how to make the trails from the **Platformer Mod: Add Trails** appear when you go over a Speed Pad from **Platformer Mod: Add Speed and Bounce Pads**?
