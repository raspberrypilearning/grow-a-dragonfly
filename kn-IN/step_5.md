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

**Dragonfly**ನ್ನು ಆಯ್ಕೆ ಮಾಡಿ ಮತ್ತು `when flag clicked`{:class="block3events"}ದಿಂದ ಶುರುವಾಗುವ ಬರಹವನ್ನು ಹುಡುಕಿ.

Drag an `if`{:class="block3control"} inside the `forever`{:class="block3control"} block. The blocks inside the `forever`{:class="block3control"} will move inside the `if`{:class="block3control"}.

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
--- /task ---

--- task ---

Then drag a `not`{:class="block3operators"} block into the `if`{:class="block3control"} and a `touching (mouse-pointer)`{:class="block3sensing"} inside that.

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

--- /task ---

--- task ---

**ಪರೀಕ್ಷೆ:** ಹಠಾತ್ ನಿಲ್ಲುವಿಕೆ ಸರಿಯಾಗಿದೆಯೇ ಮತ್ತು ಡ್ರಾಗನ್‌ಫ್ಲೈ ಅದು `not`{:class="block3operators"} `touching (mouse-pointer)`{:class="block3sensing"} ಆದಾಗ ಮಾತ್ರ ಚಲಿಸುತ್ತದೆ ಎಂದು ಪರಿಶೀಲಿಸಿ.

--- /task ---

--- task ---

Try a different condition that makes the dragonfly move when it is far enough from the mouse-pointer:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

--- /task ---

--- save ---
