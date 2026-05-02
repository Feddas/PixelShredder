Official information on using learn.unity.com/project/2d-platformer-template has been mostly deleted. As described on https://learn.unity.com/g/2d-platformer-creators .

1. List of all mods: https://web.archive.org/web/20230611003114/https://learn.unity.com/project/2d-platformer-template
2. [Modify Tilemap](#modify-tilemap)
3. [Modify Triggers](#modify-triggers)

# Modify Tilemap

Archived from https://web.archive.org/web/20230605020247/https://learn.unity.com/tutorial/2d-platformer-challenge-paint-your-level?uv=2019.3&projectId=5c8838feedbc2a0ee1e7e030#5c8932f9edbc2a1410354fda

# Modify Triggers

Archived from https://web.archive.org/web/20230605005307mp_/https://learn.unity.com/tutorial/platformer-mod-custom-triggers?uv=2019.3&projectId=5c8838feedbc2a0ee1e7e030

Summary: Triggers are a powerful part of Unity and game development. Learn how to hook-up your own custom trigger to activate a confetti celebration!
Micro-Games: Platformer
Last updated: April 17, 2023

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

Extra Credit - Stretch your Unity skills with these additional mini-mods.
- Add more **Confetti Triggers** around the track.
- Have multiple **Confetti Celebrations** activate on one trigger.
- Use different effects for the triggers - see the **Platformer Mod: Bouncy Sparkly!** for different effects you can use.
- Triggers are very powerful - you can make all sorts of cool stuff happen! Can you figure out how to make the trails from the **Platformer Mod: Add Trails** appear when you go over a Speed Pad from **Platformer Mod: Add Speed and Bounce Pads**?
