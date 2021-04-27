## Set the scene

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Add an introductory sentence. What will learners achieve by the end of this step?
</div>
<div>
Image, gif or video showing what they will achieve by the end of the step. ![](images/image.png){:width="300px"}
</div>
</div>

--- task ---

Open a [new Scratch project](http://rpf.io/scratch-new){:target="_blank"} and delete the cat sprite. Scratch will open in another browser tab.

[[[working-offline]]]

--- /task ---

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
We use <span style="color: #0faeb0">**Dragonflies**</span> can be found all over the world and have been around for over 300 million years!</p>

--- task ---

**Choose:** Click 'Choose a Backdrop' and add a backdrop of your choice. We used the 'Jurassic' backdrop.

![](images/choose-backdrop-icon.png)

![The Stage showing the Jurassic backdrop.](images/Jurassic-backdrop.png)

--- /task ---

--- task ---

Click 'Choose a Sprite' and search for 'dragonfly' then add the **Dragonfly** sprite.

![](images/choose-sprite-icon.png)

![The search box with 'dragonfly' typed in and the Dragonfly sprite in the gallery.](images/dragonfly-search.png)

--- /task ---

--- task ---

Add a script to make the Dragonfly follow the mouse pointer (or your finger):

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
point towards (mouse-pointer v)
move [5] steps
end
```
--- /task ---

--- task ---

**Test:** Click the green flag and make the Dragonfly move around the Stage. Is the Dragonfly moving as you'd expect?

--- /task ---

The Dragonfly costume is not facing to the right so the wrong part of the Dragonfly is pointing towards the mouse.

--- task ---

Click on the **Costumes** tab and use the **Select** (arrow) tool to highlight the costume. Use the rotation arrows at bottom of the highlighted costume to turn the Dragonfly costume to the right.

![](images/rotated-costume.gif)

![](images/rotated-costume.png)

--- /task ---

Dragonfly wings make a fluttering sound as they vibrate. You can edit a sound in Scratch to create a new one.

--- task ---
Add the 'Crank' sound to the Dragonfly sprite.

[[[generic-scratch3-sound-from-library]]]

![](images/crank-sound-editor.png)

Click the 'play' button so you can hear the sound.

--- /task ---

The 'Crank' sound is too long and too slow for Dragonfly wings.

--- task ---

Select the end of the sound using your mouse or finger:

![](images/crank-copy-end.png)

Click 'Copy to New' to make a new sound with just the selected part.

--- /task ---

--- task ---

Rename your new sound from 'Crank2'to 'Wings'.

![](images/crank-wings-sound.png)

Play the new sound. 
--- /task ---

--- task ---
Click the 'Faster' button a few times until you like the result:

![](images/wings-faster.png)

--- /task ---

--- task ---
If you like, you can select the very end of the Wings sound and then click 'Delete' to remove it:

![](images/wings-shorter.png)

--- /task ---

--- task ---

Now add a block to play the 'Wings' sound when the Dragonfly moves:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
```
--- /task ---

--- task ---

**Test:** Try out your Dragonfly movement and sound effect.

--- /task ---

--- save ---