---
layout: project
type: project
image: img/gamejam/gamedevlogo.png
title: "UHM GameDev Game Jam: Temptation"
date: 2024-7 to 2024-12
published: true
labels:
  - Unity
  - C#
summary: "Helped develop a rouge-like dungeon crawler game alongside GameDev club members for the Fall2024 semester Game Jam."
---

<div class="text-center p-4">
  <img width="200px" src="img/gamejam/Tezcat_TitleScreen.png" class="img-thumbnail" >
</div>

I participated in UH GameDev's Game Jam in the Fall 2024 semester. We were tasked to make a game with the theme of temptation. After brainstorming, we went with the direction of a rouge-like dungeon crawler game, where players had to collect treasures and deposit them for gold/points. The theme is exercised with the idea that heavier treasures are worth more at the risk of slowing the player down. This idea of high risk, high reward tempts the player to take more risks. The project was done through Unity and as such scripted in C#.

This was my first time participating in a Game Jam let alone coding in C#. I took on a very minimal role of trying to implement a weight system for the items. At first, this system was separate from the inventory system, however, I suggested merging the two tasks in terms of implementation would make them easier. The person tasked with the inventory system did their own implementation of both systems so I focused more on the assets and the weight of the items themselves. To do this, I created a class Items with the ScriptableObjects class to easily assign weight values and other properties. Excerpt of code:

```c#
[CreateAssetMenu(menuName = "Inventory Item Data")]
public class Items : ScriptableObject
{
    public string itemName;
    public int score;
    public int weight;
    public Sprite icon;
    public GameObject prefab;
}
```

For my learnings, an obvious one would be learning how to program in C# since this was my first time. I relied heavily on videos and tutorials online to do my task. Another thing is how important communication is in such a large group project. This was evident when I suggested the merge of two task, where I and the other person on the task did not communicate a lot. In the future, I need to do better in taking the initative so that I can be on the same page as my peers. Overall, this Game Jam was a fun experience for me and I am planning on participating in more to keep polishing my skills.

The source code is private, however, a prototype of the game is located here: [Tezcat](https://uhmanoagamedev.itch.io/tezcat). The game has not been updated and bug fixes are still required.
