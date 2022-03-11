## ಸುಧಾರಿತ ಚಲನೆ

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ಮೌಸ್-ಪಾಯಿಂಟರ್‌ ಡ್ರಾಗನ್‌ಫ್ಲೈಯನ್ನು ಸ್ಪರ್ಶಿಸಿದರೆ ಡ್ರಾಗನ್‌ಫ್ಲೈ ʼಹಠಾತ್‌ ನಿಲ್ಲುತ್ತದೆʼ ಮತ್ತು ದಿಕ್ಕನ್ನು ಬಹಳ ವೇಗವಾಗಿ ಬದಲಾಯಿಸುತ್ತದೆ. ಇದನ್ನು ಸರಿಪಡಿಸಲು ನೀವು ಇನ್ನೊಂದು ಷರತ್ತನ್ನು ಪರಿಶೀಲಿಸುತ್ತೀರಿ.
</div>
<div>
![ಕೀಟ ಮತ್ತು ಡ್ರಾಗನ್‌ಫ್ಲೈ ತೋರಿಸುತ್ತಿರುವ Stage.](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

**Dragonfly** ನ್ನು ಆಯ್ಕೆ ಮಾಡಿ ಮತ್ತು `when flag clicked`{:class="block3events"}ದಿಂದ ಶುರುವಾಗುವ ಬರಹವನ್ನು ಹುಡುಕಿ.

`if`{:class="block3control"}ನ್ನು `forever`{:class="block3control"} ಬ್ಲಾಕ್‌ ಒಳಗೆ ಎಳೆಯಿರಿ ಮತ್ತು `forever`{:class="block3control"} ಒಳಗಿರುವ ಬ್ಲಾಕ್‌ಗಳು `if`{:class="block3control"} ಒಳಗೆ ಚಲಿಸುತ್ತವೆ.

ನಿಮ್ಮ ಕೋಡ್ ಈ ರೀತಿ ಕಾಣುತ್ತದೆ ಎಂಬುವುದನ್ನು ಎಚ್ಚರಿಕೆಯಿಂದ ಪರಿಶೀಲಿಸಿ:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if < > then
start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
end
```
--- /ಕಾರ್ಯ ---

--- ಕಾರ್ಯ ---

ನಂತರ `not`{:class="block3operators"} ಬ್ಲಾಕ್‌ನ್ನು `if`{:class="block3control"} ಒಳಗೆ ಎಳೆಯಿರಿ ಮತ್ತು `touching (mouse-pointer)`{:class="block3sensing"} ನ್ನು ಅದರೊಳಗೆ ಎಳೆಯಿರಿ.

ನಿಮ್ಮ ಕೋಡ್ ಈ ರೀತಿ ಕಾಣುತ್ತದೆ ಎಂಬುವುದನ್ನು ಪರಿಶೀಲಿಸಿ:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if <not <touching [mouse-pointer v] ?> > then
start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

ವಾಕ್ಯದಲ್ಲಿ ಹೇಗೆ ಮಾಡುತ್ತದೆಯೋ ಹಾಗೆ `not`{:class="block3operators"} ಬ್ಲಾಕ್‌ ಷರತ್ತನ್ನು ಅದರ ವಿರುದ್ಧಕ್ಕೆ ಪರಿವರ್ತಿಸುತ್ತದೆ.

--- /task ---

--- task ---

**ಪರೀಕ್ಷೆ:** ಹಠಾತ್ ನಿಲ್ಲುವಿಕೆ ಸರಿಯಾಗಿದೆಯೇ ಮತ್ತು ಡ್ರಾಗನ್‌ಫ್ಲೈ ಅದು `not`{:class="block3operators"} `touching (mouse-pointer)`{:class="block3sensing"} ಆದಾಗ ಮಾತ್ರ ಚಲಿಸುತ್ತದೆ ಎಂದು ಪರಿಶೀಲಿಸಿ.

ಪ್ರಯತ್ನಿಸಲು ಬೇರೆ ಷರತ್ತು:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

ಇದು ಡ್ರಾಗನ್‌ಫ್ಲೈ ಮೌಸ್-ಪಾಯಿಂಟರ್‌ನಿಂದ ಸಾಕಷ್ಟು ದೂರದಲ್ಲಿರುವಾಗಲೇ ಅದು ಚಲಿಸುವಂತೆ ಮಾಡುತ್ತದೆ.

**ಸಲಹೆ:** ನೀವು ಬೇರೆ ಸಂಗತಿಗಳನ್ನು ಪ್ರಯತ್ನಿಸುತ್ತಿರುವಾಗ ಬ್ಲಾಕ್‌ಗಳನ್ನು Code ಪ್ರದೇಶದಲ್ಲಿ ಎಲ್ಲಿಯಾದರೂ ಎಳೆದು ಅವುಗಳನ್ನು ಅಲ್ಲಿಯೇ ಬಿಡಬಹುದು.

--- /task ---

--- save ---
