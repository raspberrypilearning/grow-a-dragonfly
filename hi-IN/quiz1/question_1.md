## Quick quiz

Answer the three questions. There are hints to guide you to the correct answer.

When you have answered each question, click on **Check my answer**.

Have fun!

--- question ---
---
legend: 3 में से पहला प्रश्न
---

A project uses the **Crab** sprite and the **Jellyfish** sprite. The **Crab** sprite has this code:

![desc](images/crab-icon.png)

```blocks3
when flag clicked
if <not <touching color (#0000FF)?>> then
hide
end
```

What would need to happen for the **Crab** sprite to hide?

--- choices ---

- () **Crab** स्प्राइट को **जेJellyfish** को छूने की आवश्यकता होगी

 --- feedback ---

 नहीं, `if`{:class="block3control"} ब्लॉक में `Sensing`{:class="block3sensing"} कंडीशन है, लेकिन यह `touching Jellyfish`{:class="block3sensing"} ब्लॉक का उपयोग नहीं करता है।

 --- /feedback ---

- (x) **Crab** स्प्राइट को नीले रंग को छूने की आवश्यकता नहीं होगी

 --- feedback ---

Yes, the `not`{:class="block3operators"} operator means that the condition is true `if`{:class="block3control"} the **Crab** sprite is not `touching`{:class="block3sensing"} the colour blue.

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
