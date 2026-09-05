## ಇನ್ನಷ್ಟು ಆಹಾರ

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ಡ್ರಾಗನ್‌ಫ್ಲೈಗೆ ಕೀಟಗಳ ಆಯ್ಕೆ ಅಗತ್ಯವಿದೆ.
</div>
<div>
![ಎರಡು ಕೀಟಗಳು ಮತ್ತು ಡ್ರಾಗನ್‌ಫ್ಲೈ ಇರುವ Stage.](images/more-food.png){:width="300px"}
</div>
</div>

--- task ---

Stage ಕೆಳಗಿರುವ Sprite ಲಿಸ್ಟ್‌ನಲ್ಲಿ **Insect** ಸ್ಪ್ರೈಟ್ ಮೇಲೆ ರೈಟ್‌-ಕ್ಲಿಕ್‌ ಮಾಡಿ ಮತ್ತು ಅದನ್ನು **duplicate** ಮಾಡಿ.

![Insect ಸ್ಪ್ರೈಟ್‌ ಆಯ್ಕೆಮಾಡಿದ Sprite ಲಿಸ್ಟ್‌ ಮತ್ತು ಮೆನುನಲ್ಲಿ 'duplicate' ಹೈಲೈಟ್‌ ಆಗಿರುವುದು.](images/duplicate-insect.png)

--- /task ---

ಈ ಕೀಟವು ನೊಣಕ್ಕಿಂತ ಭಿನ್ನವಾಗಿ ಕಂಡರೆ ಅನುಕೂಲವಾಗುತ್ತದೆ.

--- task ---

**Costumes** ಟ್ಯಾಬ್‌ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ.

+ ಈ ಕೀಟದ ಬಣ್ಣವನ್ನು ಬದಲಿಸಲು **Fill** ಟೂಲ್‌ ಉಪಯೋಗಿಸಿ
+ ನಿಮ್ಮದೇ ಕೀಟದ ಉಡುಪನ್ನು **Paint** ಮಾಡಿ
+ Scratch ನಿಂದ ಇನ್ನೊಂದು ಸಣ್ಣ ಕೀಟದ ಉಡುಪನ್ನು**ಸೇರಿಸಿ**

--- /task ---

ಕೀಟವು ಡ್ರಾಗನ್‌ಫ್ಲೈನ ರೆಕ್ಕೆ ಅಥವಾ ಬಾಲವನ್ನು ಸ್ಪರ್ಶಿಸಿದರೂ ಅದು ತಿನ್ನಲ್ಪಡುತ್ತದೆ.

ಆಪ್‌ನ್ನು ಹೆಚ್ಚು ನೈಜವಾಗಿರುವಂತೆ ಮಾಡಲು, ಇದನ್ನು ಸರಿಪಡಿಸಿ, ಆಗ ಕೀಟಗಳು ಡ್ರಾಗನ್‌ಫ್ಲೈ ಬಾಯಿಯಿಂದ ತಿನ್ನಲ್ಪಡುತ್ತವೆ. ನೀವು `touching color`{:class="block3sensing"} ಬ್ಲಾಕ್‌ ಉಪಯೋಗಿಸಬಹುದು, ಆಗ ಕೀಟವು **Dragonfly** ಮೇಲೆ ನಿರ್ದಿಷ್ಟ ಬಣ್ಣವನ್ನು ಸ್ಪರ್ಶಿಸಿದರೆ ಮಾತ್ರ ಅದು ತಿನ್ನಲ್ಪಡುತ್ತದೆ.

--- task ---

**Dragonfly** ಸ್ಪ್ರೈಟ್‌ ಆಯ್ಕೆ ಮಾಡಿ ಮತ್ತು **Costumes** ಟ್ಯಾಬ್‌ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ.

**Dragonfly**ನ ಬಾಯಿಯನ್ನು ಭರ್ತಿಮಾಡಲು ಫಿಲ್‌ ಟೂಲ್‌ ಉಪಯೋಗಿಸಿ. ನಾವು ನೇರಳೆಬಣ್ಣ ಉಪಯೋಗಿಸಿದ್ದೇವೆ:

![Fill ಟೂಲ್‌ ಆಯ್ಕೆಯಾಗಿರುವ Paint ಎಡಿಟರ್‌ ಮತ್ತು ನೇರಳೆಬಣ್ಣದ ಬಾಯಿಯಿರುವ dragonfly ಉಡುಪು.](images/dragonfly-mouth-colour.png)

--- /task ---

You need to check that the new sprite is touching the **Dragonfly** sprite `and`{:class="block3operators"} touching the colour of the dragonfly's mouth.

--- task ---

Select your new sprite and click on the **Code** tab.

`and`{:class="block3operators"} ಬ್ಲಾಕ್‌ನ್ನು `if`{:class="block3control"} ಬ್ಲಾಕ್‌ ಒಳಗೆ ಎಳೆಯಿರಿ.

`and`{:class="block3operators"} ಬ್ಲಾಕ್‌ನ್ನು `if`{:class="block3control"} ಬ್ಲಾಕ್‌ ಒಳಗೆ ಎಳೆಯಿರಿ.

![](images/insect2-icon.png)

```blocks3
when flag clicked
show
forever
move [3] steps 
if on edge, bounce
+if <<touching [Dragonfly v] ?> and <>> then
broadcast [food v]
hide
go to (random position v)
show
end
end
```

--- /task ---

--- task ---

Drag a `touching color`{:class="block3sensing"} block into the other space of the `and`{:class="block3operators"} block:

```blocks3
when flag clicked
show
forever
move [3] steps
if on edge, bounce
+if <<touching [Dragonfly v] ?> and <touching color (#9966ff) ?>> then
broadcast [food v]
hide
go to (random position v)
show
end
end
```

`touching color`{:class="block3sensing"} ಬ್ಲಾಕ್‌ನ್ನು `and`{:class="block3operators"} ಬ್ಲಾಕ್‌ನ ಬಲಭಾಗಕ್ಕೆ ಎಳೆಯಿರಿ:

![ಐಡ್ರಾಪರ್‌ ಟೂಲ್‌ನೊಂದಿಗೆ ಬಣ್ಣದ ವೃತ್ತದ ಮೇನು.](images/colour-eyedropper.png)

ಅದು ಡ್ರಾಗನ್‌ಫ್ಲೈ ಬಾಯಿಯ ಆಯ್ಕೆಮಾಡಿದ ಬಣ್ಣವನ್ನು ಹೊಂದಿಲ್ಲದಿದ್ದರೆ, ಬಣ್ಣದ ವೃತ್ತದ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ ಮತ್ತು ನಂತರ ಬಣ್ಣವನ್ನು ಆಯ್ಕೆಮಾಡಲು **Eyedropper** ಟೂಲ್‌ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ.

![ಡ್ರಾಗನ್‌ಫ್ಲೈಯ ನೇರಳೆ ಬಣ್ಣದ ಬಾಯಿಯ ಮೇಲೆ ತೂಗಾಡುತ್ತಿರುವ colour select ಹೈಲೈಟರ್‌ ಇರುವ eyedropper ಟೂಲ್.](images/colour-select.png)

ಬಣ್ಣವನ್ನು ಹೊಂದಿಸಲು Stage ಮೇಲಿನ ಡ್ರಾಗನ್‌ಫ್ಲೈ ಬಾಯಿಯ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ:

--- /task ---

--- task ---

**Test:** Check the dragonfly can only eat the second insect with its mouth.

--- /task ---

--- save ---

