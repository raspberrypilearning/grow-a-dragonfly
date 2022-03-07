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

`if`{:class="block3control"} ब्लॉक `forever`{:class="block3control"} ब्लॉकच्या आत ड्रॅग करा आणि `forever`{:class="block3control"} च्या आतील ब्लॉक्स `if`{:class="block3control"} ब्लॉक्सच्या आत हलेल.

तुमचा कोड यासारखा दिसत आहे का ते काळजीपूर्वक तपासा:

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

`not`{:class="block3operators"} ब्लॉक `if`{:class="block3control"} मध्ये ड्रॅग करा आणि `touching (mouse-pointer)`{:class="block3sensing"} त्याच्या आत.

तुमचा कोड यासारखा दिसत आहे का ते तपासा:

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

`not`{:class="block3operators"} ब्लॉक एका वाक्याप्रमाणे विरूद्ध स्थितीत बदलतो.

--- /task ---

--- task ---

**चाचणी:** ग्लिच फिक्स केला का ते तपासा आणि ड्रॅगनफ्लाय केवळ तेव्हाच हलतो जेव्हा तो `not`{:class="block3operators"} `touching (mouse-pointer)`{:class="block3sensing"}.

प्रयत्न करण्यासाठी वेगळी स्थिती:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

यामुळे ड्रॅगनफ्लाय माऊस-पॉइंटरपासून पुरेसा दूर असतांना तो हलतो.

**टीप:** तुम्ही Code भागात कोठेही ब्लॉक्स ड्रॅग करू शकता आणि ते तुम्ही वेगळ्या गोष्टींचा प्रयत्न करत असतांना तेथेच सोडू शकता.

--- /task ---

--- save ---
