## ದೃಶ್ಯವನ್ನು ಹೊಂದಿಸಿ

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ನೀವು ದೃಶ್ಯವನ್ನು ಹೊಂದಿಸುವಿರಿ. ನೀವು ಹಿನ್ನೆಲೆಯನ್ನು ಆಯ್ಕೆ ಮಾಡಿಕೊಳ್ಳಿ ಮತ್ತು Stage ಸುತ್ತ ಮೌಸ್-ಪಾಯಿಂಟರ್‌ ಅನುಸರಿಸುವ ಡ್ರಾಗನ್‌ಫ್ಲೈ ಸೇರಿಸಿ.
</div>
<div>
![](images/set-the-scene.png){:width="300px"}
</div>
</div>

--- task ---

[ಡ್ರಾಗನ್‌ ಫ್ಲೈ ಬೆಳೆಸಿ ಪ್ರಾರಂಭಿಕ ಪ್ರಾಜೆಕ್ಟ್](https://scratch.mit.edu/projects/535695413/editor){:target="_blank"} ತೆರೆಯಿರಿ. Scratch will open a blank project in a new browser tab.

--- /task ---

--- task ---

Click **Choose a Backdrop** and add a backdrop of your choice. ನಾವು **Jurassic** ಹಿನ್ನೆಲೆ ಉಪಯೋಗಿಸಿದ್ದೇವೆ.

![Backdrop icon on the Scratch app interface](images/choose-backdrop-icon.png)

![Jurassic ಹಿನ್ನೆಲೆಯನ್ನು ತೋರಿಸುವ Stage.](images/Jurassic-backdrop.png)

--- /task ---

--- task ---

**Choose a Sprite** ಕ್ಲಿಕ್‌ ಮಾಡಿ ಮತ್ತು `dragonfly` ಹುಡುಕಿ, ನಂತರ **Dragonfly** ಸ್ಪ್ರೈಟ್‌ ಸೇರಿಸಿ.

![Sprite icon on the Scratch app interface](images/choose-sprite-icon.png)

!['dragonfly' ಟೈಪ್‌ ಆಗಿರುವ ಸರ್ಚ್‌ ಬಾಕ್ಸ ಮತ್ತು ಗ್ಯಾಲರಿಯಲ್ಲಿ Dragonfly ಸ್ಪ್ರೈಟ್.](images/dragonfly-search.png)

--- /task ---

--- task ---

**Dragonfly** ಸ್ಪ್ರೈಟ್‌ ಮೌಸ್-ಪಾಯಿಂಟರ್‌ (ಅಥವಾ ನಿಮ್ಮ ಬೆರಳನ್ನು) ಅನುಸರಿಸುವಂತೆ ಮಾಡಲು ಬರಹವನ್ನು ಸೇರಿಸಿ:

![Dragonfly sprite icon on the Scratch app interface](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] % // to start small
forever
point towards (mouse-pointer v)
move [5] steps
end
```
--- /task ---

--- task ---

**ಪರೀಕ್ಷೆ:** ಹಸಿರು ಬಾವುಟ ಕ್ಲಿಕ್‌ ಮಾಡಿ ಮತ್ತು **Dragonfly** ಸ್ಪ್ರೈಟ್‌ Stage ಸುತ್ತ ಚಲಿಸುವಂತೆ ಮಾಡಿ. ನೀವು ನಿರೀಕ್ಷಿಸಿದಂತೆ ಡ್ರಾಗನ್‌ಫ್ಲೈ ಚಲಿಸುತ್ತಿದೆಯೇ?

--- /ಕಾರ್ಯ ---

Dragonfly ಉಡುಪು ಬಲ ಭಾಗಕ್ಕೆ ಮುಖಮಾಡಿಲ್ಲ, ಅದರಿಂದ **Dragonfly** ಸ್ಪ್ರೈಟ್‌ನ ತಲೆ ಮೌಸ್-ಪಾಯಿಂಟರ್‌ ಕಡೆಗೆ ಸೂಚಿಸುತ್ತಿಲ್ಲ.

--- task ---

**Costumes** ಟ್ಯಾಬ್‌ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ ಮತ್ತು **Select** (ಬಾಣ) ಟೂಲ್‌ನ್ನು ಉಡುಪು ಆಯ್ಕೆ ಮಾಡಲು ಉಪಯೋಗಿಸಿ.

**Dragonfly** ಉಡುಪು ಬಲ ಭಾಗಕ್ಕೆ ಮುಖಮಾಡುವಂತೆ ತಿರುಗಿಸಲು ಆಯ್ಕೆ ಮಾಡಿದ ಉಡುಪಿನ ಕೆಳಭಾಗದಲ್ಲಿರುವ **Rotate** ಟೂಲ್‌ ಉಪಯೋಗಿಸಿ.

![ಡ್ರಾಗನ್‌ಫ್ಲೈ ಬಲಕ್ಕೆ ಮುಖಮಾಡುವಂತೆ ಮಾಡಲು ತಿರುಗುವ ಬಾಣಗಳನ್ನು ಎಳೆದು ಡ್ರಾಗನ್‌ಫ್ಲೈ ಉಡುಪನ್ನು ಹೇಗೆ ತಿರುಗಿಸಬೇಕೆಂದು ತೋರಿಸುವ ಅನಿಮೇಟೆಡ್‌ ಚಿತ್ರ.](images/rotated-costume.gif)

--- /task ---

--- task ---

**ಪರೀಕ್ಷೆ:** ಹಸಿರು ಬಾವುಟವನ್ನು ಕ್ಲಿಕ್‌ ಮಾಡಿ ಮತ್ತು ಈಗ ಡ್ರಾಗನ್‌ಫ್ಲೈ ಹೇಗೆ ಚಲಿಸುತ್ತದೆ ಎಂದು ನೋಡಿ.

--- /task ---

ಡ್ರಾಗನ್‌ಫ್ಲೈ ರೆಕ್ಕೆಗಳು ಕಂಪಿಸಿದಾಗ ರೆಕ್ಕೆಬಡಿತದ ಶಬ್ದ ಮಾಡುತ್ತವೆ. Scratchನಲ್ಲಿ ನೀವು ನಿಮ್ಮದೇ ಧ್ವನಿಯನ್ನು ರಚಿಸಲು ಧ್ವನಿಯನ್ನು ಎಡಿಟ್‌ ಮಾಡಬಹುದು.

--- task ---

**Crank** ಧ್ವನಿಯನ್ನು **Dragonfly** ಸ್ಪ್ರೈಟ್‌ಗೆ ಸೇರಿಸಿ.

[[[generic-scratch3-sound-from-library]]]

![](images/crank-sound-editor.png)

--- /task ---

--- task ---

**Play** ಬಟನ್‌ ಕ್ಲಿಕ್‌ ಮಾಡಿ ನೀವು ಧ್ವನಿಯನ್ನು ಕೇಳಬಹುದು.

--- /task ---

**Crank** ಧ್ವನಿಯು ಡ್ರಾಗನ್‌ಫ್ಲೈ ರೆಕ್ಕೆಗಳಿಗೆ ಬಹಳ ಉದ್ದ ಮತ್ತು ನಿಧಾನವಾಗಿದೆ.

--- task ---

ನಿಮ್ಮ ಕರ್ಸರ್‌ ಅಥವಾ ಬೆರಳನ್ನು ಉಪಯೋಗಿಸಿಕೊಂಡು ಧ್ವನಿಯ ಅಂತ್ಯವನ್ನು ಆಯ್ಕೆ ಮಾಡಿ.

ಆಯ್ಕೆ ಮಾಡಿಕೊಂಡ ಭಾಗಕ್ಕಷ್ಟೆ ಹೊಸ ಧ್ವನಿಯನ್ನು ಮಾಡಲು **Copy to New** ಕ್ಲಿಕ್‌ ಮಾಡಿ:

![ಆಯ್ಕೆ ಮಾಡಿದ crank ಧ್ವನಿಯ ತುದಿ ನೀಲಿ ಬಣ್ಣದಲ್ಲಿದೆ ಮತ್ತು 'Copy to New' ಐಕಾನ್‌ ಹೈಲೈಟ್‌ ಆಗಿದೆ.](images/crank-copy-end.png)

--- /task ---

--- task ---

ನಿಮ್ಮ ಹೊಸ ಧ್ವನಿಯನ್ನು **Crank2**ದಿಂದ `Wings` ಎಂದು ಮರುನಾಮಕರಣ ಮಾಡಿ. ![Sound ಗುಣಲಕ್ಷಣವನ್ನು rename‌ ಮಾಡಿ.](images/crank-wings-sound.png)

--- /task ---

--- task ---

**Test:** Play the new sound. Click the **Faster** button a few times until you like the result:

![A faster sound wave with the 'Faster' icon highlighted.](images/wings-faster.png)

--- /task ---

--- task ---

If you like, you can select the very end of the **Wings** sound, and then click **Delete** to remove it:

![The end of the sound wave selected with the 'Delete' tool highlighted.](images/wings-shorter.png)

--- /task ---

--- task ---

Now add a block to play the **Wings** sound when the dragonfly moves:

![Dragonfly sprite icon](images/dragonfly-icon.png)

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

**Test:** Try out your dragonfly movement and sound effect.

--- /task ---

--- save ---
