## कीटकाची कुठेही हालचाल

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
तुमच्या ऍपमधील कीटक अगदी अंदाज लावता येण्याजोग्या पॅटर्नमध्ये फिरतात, परंतु वास्तविक जीवनात त्यांना पकडणे कठीण आहे. 

कीटक जास्त नैसर्गीक पद्धतीने हलण्यासाठी तुम्ही `pick random`{:class="block3operators"} ब्लॉक वापराल.
</div>
<div>
![वेगवेगळ्या दिशांना दिशा दाखवणारे कीटक दाखवणारा Stage.](images/random-movement.png){:width="300px"}
</div>
</div>

--- task ---

त्याला प्रत्येक 1-3 सेकंदांनी कुठल्याही दिशेत दाखवण्यासाठी **Insect 2** मध्ये स्क्रिप्ट जोडा.

--- /task ---

--- task ---

**चाचणी:** तुमचा प्रोजेक्ट रन कराआणि माशी कशी फिरते ते पहा. तुम्हाला हवा असलेला प्रभाव मिळविण्यासाठी संख्या बदलण्याचा प्रयत्न करा.

--- /task ---

--- task ---

Change the first **Insect** so that it can only be eaten with the dragonfly's mouth.

--- /task ---

### Add more insects

त्यांना जलद किंवा हळू करण्यासाठी तुम्ही `move`{:class="block3motion"} होणाऱ्या टप्प्यांची संख्या बदलू शकता.

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

त्याला प्रत्येक 1-3 सेकंदांनी कुठल्याही दिशेत दाखवण्यासाठी **Insect 2** मध्ये स्क्रिप्ट जोडा.

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
