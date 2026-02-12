## విశ్లేషణ

Answer the three questions. There are hints to guide you to the correct answer.

మీరు `Events`{:class="block3events"}, `Control`{:class="block3control"}, `Sensing`{:class="block3sensing"}, `Operators`{:class="block3operators"}, `Motion`{:class="block3motion"}, `Looks`{:class="block3looks"}, మరియు `Sound`{:class="block3sound"} బ్లాక్‌లని ఉపయోగించారు!

ఇప్పుడు, విశ్లేషించే సమయం వచ్చింది — విశ్లేషించడం అనేది నేర్చుకోవడంలో ముఖ్యమైన భాగం, ఎందుకంటే ఇది మీ మెదడులో కొత్త కనెక్షన్‌లను ఏర్పరచడంలో సహాయపడుతుంది.

--- question ---
---
legend: 3లో 1వ ప్రశ్న
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

- () **Crab** sprite **Jellyfish**ని తాకాలి

 --- feedback ---

 కాదు, `if`{:class="block3control"} బ్లాక్‌ లో `Sensing`{:class="block3sensing"} షరతు ఉంది, కానీ అది `touching Jellyfish`{:class="block3sensing"} బ్లాక్‌ని ఉపయోగించదు.

 --- /feedback ---

- (x) **Crab** sprite నీలం రంగును తాకకూడదు

 --- feedback ---

Yes, the `not`{:class="block3operators"} operator means that the condition is true `if`{:class="block3control"} the **Crab** sprite is not `touching`{:class="block3sensing"} the colour blue.

 --- /feedback ---

- () **Crab** sprite నీలం రంగును తాకాలి

 --- feedback ---

 నిజానికి కాదు, `operator`{:class="block3operators"}ని దగ్గరగా చూడండి.

 --- /feedback ---

- ( )`when the flag is clicked`{:class="block3events"} **Crab** sprite`hide`{:class="block3looks"} అవుతుంది

 --- feedback ---

 లేదు, **Crab** sprite కోడ్ లో `if`{:class="block3control"} బ్లాక్ ఉంది కాబట్టి అది షరతుకు అనుగుణంగా ఉంటే మాత్రమే దాచబడుతుంది.

 --- /feedback ---

--- /choices ---

--- /question ---
