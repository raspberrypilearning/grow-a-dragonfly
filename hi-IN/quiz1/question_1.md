## सोचिए

बहुत बढ़िया, आपने उपयोगकर्ता द्वारा नियंत्रित ड्रैगनफ्लाई और एल्गोरिथम का पालन करने वाले कीड़ों के साथ एक प्रकृति ऐप बनाया!

आपने `Events`{:class="block3events"}, `Control`{:class="block3control"}, `Sensing`{:class="block3sensing"}, `Operators`{:class="block3operators"}, `Motion`{:class="block3motion"}, `Looks`{:class="block3looks"}, and `Sound`{:class="block3sound"} ब्लॉक का इस्तेमाल किया है!

अब चिंतन करने का समय है - चिंतन करना सीखने का एक महत्वपूर्ण हिस्सा है, क्योंकि यह आपके मस्तिष्क में नए संबंध बनाने में मदद करता है।

आपने जो सीखा है उस पर चिंतन करने के लिए नीचे दिए गए तीन प्रश्नों के उत्तर दें।

प्रत्येक प्रश्न के बाद, सबमिट करें दबाएं। यह आपको सही उत्तर की तरफ लेकर जाएगा। आप इस गतिविधि को जितनी बार चाहें उतनी बार कर सकते हैं।

मजे करें!

--- question ---
---
legend: 3 में से पहला प्रश्न
---

एक प्रोजेक्ट **Crab** स्प्राइट और **Jellyfish** स्प्राइट का उपयोग करता है। **Crab** स्प्राइट का यह कोड है:

![विवरण](images/crab-icon.png)

```blocks3
when flag clicked
if <not <touching color (#0000FF)?>> then
hide
end
```

**Crab** स्प्राइट छिप जाए ऐसा होने के के लिए क्या होना होगा?

--- choices ---

- () **Crab** स्प्राइट को **जेJellyfish** को छूने की आवश्यकता होगी

 --- feedback ---

 नहीं, `if`{:class="block3control"} ब्लॉक में `Sensing`{:class="block3sensing"} कंडीशन है, लेकिन यह `touching Jellyfish`{:class="block3sensing"} ब्लॉक का उपयोग नहीं करता है।

 --- /feedback ---

- (x) **Crab** स्प्राइट को नीले रंग को छूने की आवश्यकता नहीं होगी

 --- feedback ---

हां, `not`{:class="block3operators"} ऑपरेटर का मतलब है कि कंडीशन सही है `if`{:class="block3control"} **Crab** स्प्राइट रंग नीले को `touching` {:class="block3sensing"} नहीं है।

 --- /feedback ---

- () **Crab** स्प्राइट को नीले रंग को छूने की आवश्यकता नहीं होगी

 --- feedback ---

 पूरी तरह से नहीं, कंडीशन में `ऑपरेटर`{:class="block3operators"} स्थिति को करीब से देखें।

 --- /feedback ---

- ( ) `when the flag is clicked`{:class="block3events"} **Crab** स्प्राइट हमेशा `hide`{:class="block3looks"} करेगा

 --- feedback ---

 नहीं, **Crab** स्प्राइट के कोड में एक `if`{:class="block3control"} ब्लॉक है, इसलिए यह केवल तभी छिपा होगा जब कंडीशन पूरी हो।

 --- /feedback ---

--- /choices ---

--- /question ---
