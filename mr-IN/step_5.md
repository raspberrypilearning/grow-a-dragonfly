## सुधारित हालचाल

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ड्रॅगनफ्लाय "ग्लिच" करतो आणि माऊस-पॉइंटर ड्रॅगनफ्लायला स्पर्श करत असल्यास तो खरोखर जलद दिशा बदलतो. हे ठीक करण्यासाठी तुम्ही दुसरी स्थिती तपासाल.
</div>
<div>
![कीटक आणि ड्रॅगनफ्लाय दाखवणारा Stage.](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

**Dragonfly** निवडा आणि `when flag clicked`{:class="block3events"} ने चालू होणारी स्क्रिप्ट शोधा.

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

**चाचणी:** ग्लिच फिक्स केला का ते तपासा आणि ड्रॅगनफ्लाय केवळ तेव्हाच हलतो जेव्हा तो `not`{:class="block3operators"} `touching (mouse-pointer)`{:class="block3sensing"}.

--- /task ---

--- task ---

Try a different condition that makes the dragonfly move when it is far enough from the mouse-pointer:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

--- /task ---

--- save ---
