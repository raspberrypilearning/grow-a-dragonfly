## अधिक भोजन

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ड्रैगनफ्लाई को कीड़ों के विकल्प की आवश्यकता होती है।
</div>
<div>
![ दो कीड़ों और ड्रैगनफ्लाई के साथ Stage।](images/more-food.png){:width="300px"}
</div>
</div>

--- task ---

Stage के तहत Sprite सूची में **Insect** स्प्राइट पर राइट-क्लिक करें और **duplicate** करें ।

![मेनू में कीट स्प्राइट के साथ Sprite सूची चयनित और 'डुप्लिकेट' हाइलाइट किया गया।](images/duplicate-insect.png)

--- /task ---

यह मददगार होगा अगर यह कीट मक्खी से अलग दिखता है।

--- task ---

**Costumes** टैब पर क्लिक करें।

+ इस कीट का रंग बदलने के लिए **Fill**> टूल का उपयोग करें
+ अपनी खुद की कीट पोशाक **Paint** करें
+ Scratch से और बग पोशाक **Add** करें

--- /task ---

अगर कीट ड्रैगनफ्लाई के पंख या पूंछ को छूता भी है तो ड्रैगनफ्लाई उसे खा जाती है।

अपने ऐप को और अधिक यथार्थवादी बनाने के लिए, इसे ठीक करें ताकि ड्रैगनफ्लाई कीट को मूँह से खाए। आप `touching color`{:class="block3sensing"} ब्लॉक का उपयोग कर सकते हैं ताकि कीट केवल तभी खाए जब वह **Dragonfly**पर किसी विशेष रंग को छूता है।

--- task ---

**Dragonfly** स्प्राइट चुनें और **Costumes** टैब पर क्लिक करें।

**Dragonfly** का मुंह भरने के लिए fill tool का उपयोग करें। हमने बैंगनी का इस्तेमाल किया:

![Fill टूल के साथ Paint एडिटर चयनित और बैंगनी मुंह वाली ड्रैगनफ्लाई पोशाक।](images/dragonfly-mouth-colour.png)

--- /task ---

You need to check that the new sprite is touching the **Dragonfly** sprite `and`{:class="block3operators"} touching the colour of the dragonfly's mouth.

--- task ---

Select your new sprite and click on the **Code** tab.

`and`{:class="block3operators"} ब्लॉक को `if`{:class="block3control"} ब्लॉक में खीचें।

`and`{:class="block3operators"} ब्लॉक को `if`{:class="block3control"} ब्लॉक में खीचें।

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

`touching color`{:class="block3sensing"} ब्लॉक को `and`{:class="block3operators"} ब्लॉक के दाईं ओर खींचें:

![आईड्रॉपर टूल के साथ कलर सर्कल मेन्यू।](images/colour-eyedropper.png)

अगर इसमें ड्रैगनफ्लाई के मुंह का रंग नहीं चुना गया है, तो रंग सर्कल पर क्लिक करें और फिर रंग चुनने के लिए **Eyedropper** टूल पर क्लिक करें।

![ड्रैगनफ्लाई के बैंगनी मुंह पर मँडराते हुए कलर सिलेक्ट हाइलाइटर के साथ आईड्रॉपर टूल।](images/colour-select.png)

रंग को मिलान के लिए सेट करने के लिए Stage पर ड्रैगनफ्लाई के मुंह पर क्लिक करें:

--- /task ---

--- task ---

**Test:** Check the dragonfly can only eat the second insect with its mouth.

--- /task ---

--- save ---

