## విశ్లేషణ

బాగా చేసారు, మీరు యూజర్ చే నియంత్రించబడే తూనీగతో మరియు అల్గారిథమ్‌ను అనుసరించే కీటకాలతో ప్రకృతి యాప్‌ని సృష్టించారు!

మీరు `Events`{:class="block3events"}, `Control`{:class="block3control"}, `Sensing`{:class="block3sensing"}, `Operators`{:class="block3operators"}, `Motion`{:class="block3motion"}, `Looks`{:class="block3looks"}, మరియు `Sound`{:class="block3sound"} బ్లాక్‌లని ఉపయోగించారు!

ఇప్పుడు, విశ్లేషించే సమయం వచ్చింది — విశ్లేషించడం అనేది నేర్చుకోవడంలో ముఖ్యమైన భాగం, ఎందుకంటే ఇది మీ మెదడులో కొత్త కనెక్షన్‌లను ఏర్పరచడంలో సహాయపడుతుంది.

మీరు నేర్చుకున్న వాటిని పరిశీలించడానికి దిగువ మూడు ప్రశ్నలకు సమాధానం ఇవ్వండి.

ప్రతి ప్రశ్న తర్వాత, సబ్మిట్ నొక్కండి. మీరు సరైన సమాధానం వైపు మార్గనిర్దేశం చేయబడతారు. మీరు ఈ చర్యను మీకు కావలసినన్ని సార్లు చేయవచ్చు.

ఆస్వాదించండి!

--- question ---
---
legend: 3లో 1వ ప్రశ్న
---

ఒక ప్రాజెక్ట్ **Crab** sprite మరియు **Jellyfish** sprite లను ఉపయోగిస్తుంది. **Crab** sprite ఈ కోడ్‌ని కలిగి ఉంది:

![desc](images/crab-icon.png)

```blocks3
when flag clicked
if <not <touching color (#0000FF)?>> then
hide
end
```

**Crab** sprite దాగడానికి ఏమి జరగాలి?

--- choices ---

- () **Crab** sprite **Jellyfish**ని తాకాలి

 --- feedback ---

 కాదు, `if`{:class="block3control"} బ్లాక్‌ లో `Sensing`{:class="block3sensing"} షరతు ఉంది, కానీ అది `touching Jellyfish`{:class="block3sensing"} బ్లాక్‌ని ఉపయోగించదు.

 --- /feedback ---

- (x) **Crab** sprite నీలం రంగును తాకకూడదు

 --- feedback ---

అవును, `not`{:class="block3operators"} ఆపరేటర్ అంటే కండిషన్ ట్రూ అని అర్థం. `if`{:class="block3control"} **Crab** sprite `not touching`{:class="block3sensing"} ఉంటే నీలం రంగు.

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
