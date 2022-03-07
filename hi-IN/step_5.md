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

एक `if`{:class="block3control"} को `forever`{:class="block3control"} ब्लॉक के अंदर खींचें और `forever`{:class="block3control"} के अंदर के ब्लॉक `if`{:class="block3control"} के अंदर चले जाएंगे।

ध्यान से जांचें कि आपका कोड इस तरह दिखता है:

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

फिर एक `not`{:class="block3operators"} ब्लॉक को `if`{:class="block3control"} में खींचें और एक `touching (mouse-pointer)`{:class="block3sensing"} को उसके अंदर खींचें।

जांचें कि आपका कोड इस तरह दिखता है:

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

`not`{:class="block3operators"} ब्लॉक एक कंडीशन को इसके विपरीत में बदल देता है, ठीक वैसे ही जैसे यह एक वाक्य में करेगा।

--- /task ---

--- task ---

**परीक्षण:** जाँच करें कि गड़बड़ ठीक हो गई है, और ड्रैगनफ्लाई केवल तभी चलती है जब वह `not`{:class="block3operators"} `touching (mouse-pointer)`{:class="block3sensing"} होती है।

आज़माने के लिए एक अलग कंडीशन है:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

यह माउस-पॉइंटर से काफी दूर होने पर ड्रैगनफ्लाई को आगे बढ़ाता है।

**सलाह:** आप ब्लॉक को Code क्षेत्र में कहीं भी खींच सकते हैं और अलग-अलग चीजों को आजमाने के दौरान उन्हें वहीं छोड़ सकते हैं।

--- /task ---

--- save ---
