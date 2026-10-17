## बेहतर गतिविधि

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
यदि माउस-पॉइंटर ड्रैगनफ्लाई को छू रहा है तो ड्रैगनफ्लाई 'झटके लेता है' और दिशा वास्तव में तेजी से बदलता है। इसे ठीक करने के लिए आप एक और कंडीशन की जांच करेंगे।
</div>
<div>
![एक कीट और ड्रैगनफ्लाई दिखाने वाला Stage।](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

**Dragonfly** का चयन करें और उस स्क्रिप्ट को खोजें जो `when flag clicked`{:class="block3events"} से शुरू होती है।

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

**परीक्षण:** जाँच करें कि गड़बड़ ठीक हो गई है, और ड्रैगनफ्लाई केवल तभी चलती है जब वह `not`{:class="block3operators"} `touching (mouse-pointer)`{:class="block3sensing"} होती है।

--- /task ---

--- task ---

Try a different condition that makes the dragonfly move when it is far enough from the mouse-pointer:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

--- /task ---

--- save ---
