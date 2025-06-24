## Challenge

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Modifie les insectes jusqu'à ce qu'ils se comportent comme tu le souhaites.
</div>
<div>
![Scène montrant des insectes pointant dans différentes directions.](images/random-movement.png){:width="300px"}
</div>
</div>

--- task ---

Change the speed of the dragonfly.

--- /task ---

--- task ---

Change the size that the dragonfly needs to grow to reach full size.

--- /task ---

--- task ---

Change the first **Insect** so that it can only be eaten with the dragonfly's mouth.

--- /task ---

### Add more insects

You can paint your own insects or trying adding an emoji mosquito!

--- task ---

Use the emoji keyboard to add a **Mosquito emoji** sprite.

Duplicate an existing **insect** sprite then click on the **Costumes** tab. **Paint** a new costume and select the **Text** tool. Instead of typing text, use the emoji keyboard shortcut for your Operating System:

- Windows - <kbd>⊞ Win</kbd> + <kbd>.</kbd>
- MacOS - <kbd>control</kbd> + <kbd>command</kbd> + <kbd>space</kbd>
- Linux - <kbd>ctrl</kbd> + <kbd>.</kbd>

![The popup emoji keyboard with the 'animals and nature' category selected.](images/emoji-keyboard.png)

Select the **Mosquito** emoji to insert it into the Paint editor. Use the **Select** (arrow) tool to centre, resize, and rotate your mosquito until you are happy with it.

![The mosquito emoji in the paint editor.](images/emoji-mosquito.png)

**Tip:** Emojis can look different on different computers, so they might not look the same on a tablet and a desktop computer. Some emojis aren't available on some computers, but most modern computers will support them.

--- /task ---

### Create random movement

Tu utiliseras le bloc « nombre aléatoire »{:class="block3operators"} pour faire bouger l'insecte de manière plus naturelle.

![Stage showing insects pointing in different directions.](images/random-movement.png){:width="300px"}

--- task ---

Ajoute un script à **Insecte2** pour le faire pointer dans une direction aléatoire toutes les 1 à 3 secondes.

![](images/insect2-icon.png)

```blocks3
when flag clicked
forever // Keep changing direction
point in direction (pick random [0] to [259])
wait (pick random [1] to [3]) seconds
end
```

--- /task ---

--- task ---

**Test :** Exécute ton projet et observe le mouvement de la mouche.

--- /task ---

--- task ---

Tu peux également faire glisser ce script vers le sprite **Insecte** afin qu'il se déplace également de manière aléatoire.

--- /task ---

### Share you insects

--- task ---

Use your Backpack to trade insects with your friends from their 'Grow a Dragonfly' projects.

Send the link of your project to your friend who can go inside the project, click on Backpack (the one under the code space) and drag and drop the sprite.

[[[scratch-backpack]]]

--- /task ---

--- task ---

Check each sprite and costume has a name that describes the image. This makes your project easier to understand if you come back to it later.

--- /task ---

--- task ---

Right-click on the Code area and choose **Clean up Blocks** to get Scratch to tidy your code.

--- /task ---

--- save ---
