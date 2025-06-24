## दृश्य को स्थापित करें

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
आप सीन सेट कर देंगे। अपनी पृष्ठभूमि चुनें और एक ड्रैगनफ्लाई जोड़ें जो Stage के चारों ओर माउस-पॉइंटर का अनुसरण करे।
</div>
<div>
![](images/set-the-scene.png){:width="300px"}
</div>
</div>

--- task ---

[Grow a dragonfly स्टार्टर प्रोजेक्ट](https://scratch.mit.edu/projects/535695413/editor){:target="_blank"} खोलें। Scratch will open a blank project in a new browser tab.

--- /task ---

--- task ---

Click **Choose a Backdrop** and add a backdrop of your choice. हमने **Jurassic** बैकड्रॉप का इस्तेमाल किया।

![Backdrop icon on the Scratch app interface](images/choose-backdrop-icon.png)

![Jurassic पृष्ठभूमि दिखाने वाला Stage।](images/Jurassic-backdrop.png)

--- /task ---

--- task ---

**Choose a Sprite** पर क्लिक करें, और `dragonfly` खोजें, फिर **Dragonfly** स्प्राइट जोड़ें।

![Sprite icon on the Scratch app interface](images/choose-sprite-icon.png)

![गैलरी में 'dragonfly' टाइप किया गया सर्च बॉक्स और Dragonfly स्प्राइट।](images/dragonfly-search.png)

--- /task ---

--- task ---

**Dragonfly** स्प्राइट को माउस-पॉइंटर (या अपनी उंगली) का अनुसरण करने के लिए एक स्क्रिप्ट जोड़ें:

![Dragonfly sprite icon on the Scratch app interface](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] % // to start small
forever
point towards (mouse-pointer v)
move [5] steps
end
```
--- /task ---

--- task ---

**परीक्षण:** हरी झंडी पर क्लिक करें और **Dragonfly** स्प्राइट को Stage के चारों ओर घुमाएँ। क्या ड्रैगनफ्लाई आपकी अपेक्षा के अनुरूप हिल रही है?

--- /task ---

ड्रैगनफ्लाई पोशाक दाईं ओर के मुख नहीं है, इसलिए **Dragonfly** स्प्राइट का सिर माउस-पॉइंटर की दिशा की ओर नहीं है।

--- task ---

**Costumes** टैब पर क्लिक करें और पोशाक का चयन करने के लिए **Select** (तीर) उपकरण का उपयोग करें।

**Dragonfly** पोशाक का मूह दाईं ओर मोड़ने के लिए चयनित पोशाक के नीचे **Rotate** उपकरण का उपयोग करें।

![एक एनिमेटेड छवि यह दिखाते हुए कि घूर्णन तीरों को खींचकर ड्रैगनफ्लाई पोशाक को कैसे घुमाया जाए ताकि ड्रैगनफ्लाई दाहिने तरफ की ओर मुंह करे ।](images/rotated-costume.gif)

--- /task ---

--- task ---

**परीक्षण:** हरे झंडे पर क्लिक करें और देखें कि ड्रैगनफ्लाई अब कैसे चलती है।

--- /task ---

ड्रैगनफ्लाई पंख कंपन करते समय एक फड़फड़ाहट की आवाज करते हैं। आप अपनी खुद की ध्वनि बनाने के लिए Scratch में ध्वनि संपादित कर सकते हैं।

--- task ---

**Dragonfly** स्प्राइट में **Crank** ध्वनि जोड़ें।

[[[generic-scratch3-sound-from-library]]]

![](images/crank-sound-editor.png)

--- /task ---

--- task ---

**Play** बटन क्लिक करें ताकि आप ध्वनि सुन सकें।

--- /task ---

**Crank** ध्वनि ड्रैगनफ्लाई पंखों के लिए बहुत लंबी और बहुत धीमी है।

--- task ---

अपने कर्सर या उंगली का उपयोग करके ध्वनि के अंत का चयन करें।

केवल चयनित भाग के साथ एक नई ध्वनि बनाने के लिए **Copy to New** पर क्लिक करें:

!['Copy to New' चिह्न के साथ नीले रंग में चयनित क्रैंक ध्वनि का अंत हाइलाइट किया गया।](images/crank-copy-end.png)

--- /task ---

--- task ---

अपनी नई ध्वनि का नाम **Crank2** से `Wings` में बदलें। ![नाम बदलने का ध्वनि गुण।](images/crank-wings-sound.png)

--- /task ---

--- task ---

**Test:** Play the new sound. Click the **Faster** button a few times until you like the result:

![A faster sound wave with the 'Faster' icon highlighted.](images/wings-faster.png)

--- /task ---

--- task ---

If you like, you can select the very end of the **Wings** sound, and then click **Delete** to remove it:

![The end of the sound wave selected with the 'Delete' tool highlighted.](images/wings-shorter.png)

--- /task ---

--- task ---

Now add a block to play the **Wings** sound when the dragonfly moves:

![Dragonfly sprite icon](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
```
--- /task ---

--- task ---

**Test:** Try out your dragonfly movement and sound effect.

--- /task ---

--- save ---
