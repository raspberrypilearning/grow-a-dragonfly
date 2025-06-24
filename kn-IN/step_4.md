## ಪೂರ್ಣ ಗಾತ್ರಕ್ಕೆ ಬೆಳೆಸಿರಿ

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ಡ್ರಾಗನ್‌ಫ್ಲೈ ನೋಣವನ್ನು ತಿಂದಾಗ ಅದು ಬೆಳೆಯುವಂತೆ ನೀವು ಮಾಡುತ್ತೀರಿ ಮತ್ತು ಅದು ಪೂರ್ಣ ಗಾತ್ರವನ್ನು ತಲುಪಿದರೆ ನಿಲ್ಲಿಸುತ್ತೀರಿ.
</div>
<div>
![Stage ಮೇಲಿನ ಪೂರ್ಣ-ಗಾತ್ರದ ಡ್ರಾಗನ್‌ಫ್ಲೈ 'I got to full size!' ಹೇಳುತ್ತಿರುವುದು.](images/grow-to-fullsize.png){:width="300px"}
</div>
</div>

ಜೀವಿಸಿರುವ ಅತ್ಯಂತ ದೊಡ್ಡ ಡ್ರಾಗನ್‌ಫ್ಲೈಗಳು ಮಧ್ಯ ಅಮೇರಿಕಾದಲ್ಲಿ ಕಂಡುಬರುತ್ತವೆ ಮತ್ತು ಅವುಗಳ ರೆಕ್ಕೆಗಳ ಅಗಲ 19ಸೆಂಮೀ ಇರುತ್ತದೆ (ನಿಮ್ಮ ಕೈಗಿಂತ ಸ್ವಲ್ಪ ದೊಡ್ಡದು). ಇದುವರೆಗೆ ತಿಳಿದಿರುವ ಅತಿದೊಡ್ಡ ಕೀಟವೆಂದರೆ <span style="color: #0faeb0">**ಮೆಗಾನ್ಯೂರೋಪ್ಸಿಸ್ ಪರ್ಮಿಯಾನಾ**</span>, ಸುಮಾರು 75ಸೆಂಮೀ ರೆಕ್ಕೆ ಅಗಲ ಹೊಂದಿರುವ ಡ್ರಾಗನ್‌ಫ್ಲೈ (ಒಂದು ದೊಡ್ಡ ಹೆಜ್ಜೆಗುರುತಿನ ಗಾತ್ರ).

ಎನಾದರೂ ಸಂಭವಿಸಿದೆ ಎಂದು ಇನ್ನೊಂದು ಸ್ಪ್ರೈಟ್‌ಗೆ ತಿಳಿಸಬೇಕೆಂದರೆ, ನೀವು `broadcast`{:class="block3events"} ಬ್ಲಾಕ್‌ನ್ನು [Broadcasting spells](https://projects.raspberrypi.org/en/projects/broadcasting-spells){:target="_blank"}ರಲ್ಲಿ ಮಾಡಿದಂತೆ ಉಪಯೋಗಿಸಬಹುದು.

--- task ---

`broadcast`{:class="block3events"} ಬ್ಲಾಕ್‌ನ್ನು **Insect** ಸ್ಪ್ರೈಟ್‌ಗೆ ಹೊಸ ಸಂದೇಶದೊಂದಿಗೆ `food`{:class="block3events"} ಸೇರಿಸಿ:

![](images/fly-icon.png)

```blocks3
when flag clicked
show // show at the start
forever
move [3] steps
if on edge, bounce
if <touching [Dragonfly v] ?> then
+broadcast [food v]
hide
go to (random position v)
wait [1] seconds
show
end
end
```
--- /task ---

**Dragonfly** ಸ್ಪ್ರೈಟ್‌ `food`{:class="block3events"} ಸಂದೇಶವನ್ನು ಸ್ವೀಕರಿಸಿದಾಗ ಅದು ಬೆಳೆಯಬೇಕು.

--- task ---

**Dragonfly** ಸ್ಪ್ರೈಟ್‌ ಆಯ್ಕೆ ಮಾಡಿ ಮತ್ತು ಈ ಬರಹವನ್ನು ಸೇರಿಸಿ:

![](images/dragonfly-icon.png)

```blocks3 
when I receive [food v]
change size by [5]
```

--- /task ---

--- task ---

ಡ್ರಾಗನ್‌ಫ್ಲೈಗೆ **Chomp** ಧ್ವನಿಯನ್ನು ಸೇರಿಸಿ ಮತ್ತು ಕೀಟವನ್ನು ತಿಂದಾಗ ಅದನ್ನು `start`{:class="block3sound"} ಮಾಡಿ:

```blocks3 
when I receive [food v]
+start sound [Chomp v]
change size by [5]
```
--- /task ---

--- task ---

**ಪರೀಕ್ಷೆ:** ಡ್ರಾಗನ್‌ಫ್ಲೈ ಬೆಳೆಯುವುದು ಮತ್ತು ಅದು ನೋಣವನ್ನು ತಿಂದಾಗ ಚಾಂಪ್‌ ಧ್ವನಿ ಮಾಡುತ್ತದೆಯೇ ಎಂದು ಪರೀಕ್ಷಿಸಲು ನಿಮ್ಮ ಪ್ರಾಜೆಕ್ಟ್‌ನ್ನು ರನ್‌ ಮಾಡಿ.

--- /task ---

ಡ್ರಾಗನ್‌ಫ್ಲೈ ಅದರ ಪೂರ್ಣ ಗಾತ್ರವನ್ನು ತಲುಪಿದಾಗ, ಆಟವು ನಿಮಗೆ ಶುಭಾಶಯ ತಿಳಿಸುತ್ತದೆ ಮತ್ತು ನಿಂತು ಹೋಗುತ್ತದೆ.

--- task ---

`if`{:class="block3control"} ಬ್ಲಾಕ್‌ನ್ನು ಸೇರಿಸಿ.

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
+if < > then
end
```

--- /task ---

`size`{:class="block3looks"} `=`{:class="block3operators"} `100%` ಆದಾಗ ಡ್ರಾಗನ್‌ಫ್ಲೈ ಪೂರ್ಣ-ಗಾತ್ರದ್ದಾಗುತ್ತದೆ.

--- task ---

First, add an `=`{:class="block3operators"} operator into the hexagon-shaped input:

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
+if <[ ] = [ ]> then
end
```
--- /task ---

--- task ---

ಅಂತರ್ನಿರ್ಮಿತ `size`{:class="block3looks"} ವೇರಿಯೇಬಲ್‌ ಸೇರಿಸಿ ಷರತ್ತು ರಚನೆಯನ್ನು ಮುಗಿಸಿ ಮತ್ತು ಮೌಲ್ಯ `100`ನ್ನು ಟೈಪ್‌ ಮಾಡಿ:

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
+if <(size) = [100]> then
end
```
--- /task ---

--- task ---

ಬ್ಲಾಕ್‌ಗಳನ್ನು ಸೇರಿಸಿ, ಅದರಿಂದ `if`{:class="block3control"} ಷರತ್ತು ಸರಿ ಆದರೆ `then`{:class="block3control"} ಡ್ರಾಗನ್‌ಫ್ಲೈ 'end' ಸಂದೇಶ `broadcast`{:class="block3events"} ಮಾಡುತ್ತದೆ ಮತ್ತು `say`{:class="block3looks"} `I got to full size!`

ಅಂತಿಮವಾಗಿ, ಉಳಿದ ಡ್ರಾಗನ್‌ಫ್ಲೈ ಬರಹಗಳನ್ನು ನಿಲ್ಲಿಸಲು `stop all`{:class="block3control"} ಬ್ಲಾಕ್‌ ಸೇರಿಸಿ:

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
if <(size) = [100]> then
+broadcast [end v]
+say [I got to full size!]
+stop [other scripts in sprite v] // change from 'all'
end
```
--- /task ---

--- task ---

ಈ ಸಮಯದಲ್ಲಿ, ಪ್ರಾಜೆಕ್ಟ ಮುಗಿದ ನಂತರವೂ ನೊಣ ಚಲಿಸುತ್ತದೆ. ಈ ಬರಹವನ್ನು **Insect** ಸ್ಪ್ರೈಟ್‌ಗೆ ಸೇರಿಸಿ.

![](images/fly-icon.png)

```blocks3
when I receive [end v]
stop [other scripts in sprite v]
```

--- /task ---

--- task ---

**ಪರೀಕ್ಷೆ:** ಹಸಿರು ಬಾವುಟವನ್ನು ಕ್ಲಿಕ್‌ ಮಾಡಿ ಮತ್ತು ನಿಮ್ಮ ಡ್ರಾಗನ್‌ಫ್ಲೈ ಪೂರ್ಣ-ಗಾತ್ರ ತಲುಪುವವರೆಗೆ ನೊಣಗಳನ್ನು ತಿನ್ನುತ್ತಲೇ ಇರಿ.

--- /task ---

--- save ---
