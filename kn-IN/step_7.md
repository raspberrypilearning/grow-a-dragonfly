## ಕೀಟದ ಯಾದೃಚ್ಛಿಕ ಚಲನೆ

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ನಿಮ್ಮ ಆಪ್‌ನಲ್ಲಿರುವ ಕೀಟಗಳು ಬಹಳ ಊಹಿಸಬಹುದಾದ ವಿನ್ಯಾಸಗಳಲ್ಲಿ ಚಲಿಸುತ್ತವೆ, ಆದರೆ ನಿಜಜೀವನದಲ್ಲಿ ಅವುಗಳನ್ನು ಹಿಡಿಯುವುದು ಕಷ್ಟ. 

ಕೀಟವು ಹೆಚ್ಚು ಸ್ವಾಭಾವಿಕ ರೀತಿಯಲ್ಲಿ ಚಲಿಸುವಂತೆ ಮಾಡಲು ನೀವು `pick random`{:class="block3operators"} ಬ್ಲಾಕ್‌ ಉಪಯೋಗಿಸುತ್ತೀರಿ.
</div>
<div>
![ಕೀಟಗಳು ಬೇರೆ ಬೇರೆ ದಿಕ್ಕುಗಳನ್ನು ಸೂಚಿಸುತ್ತಿರುವುದನ್ನು ತೋರಿಸುತ್ತಿರುವ Stage.](images/random-movement.png){:width="300px"}
</div>
</div>

--- task ---

ಪ್ರತಿ 1–3 ಸೆಕೆಂಡುಗಳಿಗೆ **Insect 2** ಯಾದೃಚ್ಛಿಕ ದಿಕ್ಕನ್ನು ಸೂಚಿಸುವಂತೆ ಮಾಡಲು ಬರಹವನ್ನು ಸೇರಿಸಿ.

--- /task ---

--- task ---

**ಪರೀಕ್ಷೆ:** ನಿಮ್ಮ ಪ್ರಾಜೆಕ್ಟ್‌ನ್ನು ರನ್‌ ಮಾಡಿ ಮತ್ತು ನೋಣ ಹೇಗೆ ಚಲಿಸುತ್ತದೆ ಎಂದು ವೀಕ್ಷಿಸಿ. ನಿಮಗೆ ಬೇಕಾದ ಪರಿಣಾಮ ಪಡೆಯಲು ಸಂಖ್ಯೆಗಳನ್ನು ಬದಲಾಯಿಸಲು ಪ್ರಯತ್ನಿಸಿ.

--- /task ---

--- task ---

Change the first **Insect** so that it can only be eaten with the dragonfly's mouth.

--- /task ---

### Add more insects

ಅವುಗಳನ್ನು ವೇಗ ಅಥವಾ ನೀಧಾನಗೊಳಿಸಲು ನೀವು ಅವುಗಳ `move`{:class="block3motion"} ಹಂತಗಳ ಸಂಖ್ಯೆಯನ್ನು ಬದಲಾಯಿಸಬಹುದು.

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

Use the `pick random`{:class="block3operators"} block to make the insect move in a more natural way.

![Stage showing insects pointing in different directions.](images/random-movement.png){:width="300px"}

--- task ---

ಪ್ರತಿ 1–3 ಸೆಕೆಂಡುಗಳಿಗೆ **Insect 2** ಯಾದೃಚ್ಛಿಕ ದಿಕ್ಕನ್ನು ಸೂಚಿಸುವಂತೆ ಮಾಡಲು ಬರಹವನ್ನು ಸೇರಿಸಿ.

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

**Test:** Run your project and watch how the sprite moves.

--- /task ---

--- task ---

Drag this script to the other **Insect** sprite to make it move randomly.

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
