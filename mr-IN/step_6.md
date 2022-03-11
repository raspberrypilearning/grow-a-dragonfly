## अधिक अन्न

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ड्रॅगनफ्लायला कीटकांच्या निवड करण्याची आवश्यकता असते.
</div>
<div>
![दोन कीटक आणि ड्रॅगनफ्लाय दाखवणारा Stage.](images/more-food.png){:width="300px"}
</div>
</div>

--- task ---

Stage अंतर्गत Sprite लीस्टमधील **Insect** स्प्राईटवर राईट-क्लिक करा आणि त्याला **duplicate** करा.

![कीटक स्प्राईटसह Sprite लीस्ट निवडलेली आहे आणि ती मेनूमध्ये 'डुप्लीकेट' हायलाइट केलेली आहे.](images/duplicate-insect.png)

--- /task ---

हा कीटक माशीपेक्षा वेगळा दिसल्यास ते फायदेशीर होईल.

--- task ---

**Costumes** टॅबवर क्लिक करा.

**निवडा:** वेगळा उडणारा कीटक तयार करा.
+ या कीटकाचा रंग बदलण्यासाठी **Fill** टूल वापरा
+ तुमचा स्वतःचा कॉश्चुम **Paint** करा
+ Scratch मधून दुसरा बग कॉश्चुम **Add** जोडा

--- /task ---

ड्रॅगनफ्लायच्या पंखाला किंवा शेपटीला स्पर्श केला तरी कीटक खाल्ला जातो.

तुमचे ऍप जास्त खरे होण्यासाठी, हे ठीक करा जेणेकरून कीटक ड्रॅगनफ्लायच्या तोंडातूनच खाल्ला जाईल. तुम्ही `touching color`{:class="block3sensing"} ब्लॉक वापरू शकता जेणेकरून जेणेकरून कीटक तेव्हाच खाल्ला जाईल जेव्हा तो **Dragonfly** वरील विशीष्ट रंगाला स्पर्श करतो.

--- task ---

**Dragonfly** sprite निवडा आणि **Costumes** टॅबवर क्लिक करा.

**Dragonfly**चे तोंड भरण्यासाठी फिल टूलचा वापर करा. आपण जांभळा वापरला:

![Fill टूलसह Paint एडिटर निवडलेला आहे आणि ड्रॅगनफ्लाय कॉश्चुम जांभळ्या तोंडाचा आहे.](images/dragonfly-mouth-colour.png)

--- /task ---

**Insect2** sprite हा **Dragonfly** sprite ला स्पर्श करत आहे का `and`{:class="block3operators"} ड्रॅगनफ्लायच्या तोंडाच्या रंगाला स्पर्श करत आहे का ते तुम्ही तपासायला हवे.

--- task ---

**Insect2** sprite निवडा आणि **Code** टॅबवर क्लिक करा.

`and`{:class="block3operators"} ब्लॉक `if`{:class="block3control"} ब्लॉकमध्ये ड्रॅग करा.

`<touching [Dragonfly v] ?>`{:class="block3sensing"} ब्लॉक पॉप आऊट करेल, तो `and`{:class="block3operators"} ब्लॉकच्या डावीकडे ड्रॅग करा:

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

`touching color`{:class="block3sensing"} ब्लॉक `and`{:class="block3operators"} ब्लॉकच्या उजवीकडे ड्रॅग करा:

![](images/insect2-icon.png)

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

ड्रॅगनफ्लायच्या तोंडाचा रंग निवडलेला नसल्यास, कलर सर्कलवर क्लिक करा आणि नंतर रंग निवडण्यासाठी **Eyedropper** टूलवर क्लिक करा.

![Eyedropper टूलसह कलर सर्कल मेनू.](images/colour-eyedropper.png)

रंग जुळण्यास रंग सेट करण्यासाठी Stage वरील ड्रॅगनफ्लायच्या तोंडावर क्लिक करा:

![ड्रॅगनफ्लायच्या जांभळ्या तोंडावर रंग निवडलेले हायलाइटर असलेले eyedropper टूल.](images/colour-select.png)

**टीप:** हे करणे अवघड असल्यास, **Dragonfly** sprite चा आकार बदला जेणेकरून ते खरोखर मोठे असेल.

--- /task ---

--- task ---

**चाचणी:** आता तपासा की, ड्रॅगनफ्लाय फक्त दुसरा कीटक त्याच्या तोंडाने खाऊ शकतो.

तुम्हाला आवडत असल्यास, तुम्ही पहिला **Insect** बदलू शकता जेणेकरून तो फक्त ड्रॅगनफ्लायच्या तोंडाने खाल्ला जाऊ शकतो.

--- /task ---

--- save ---

