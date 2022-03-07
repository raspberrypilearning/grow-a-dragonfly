
--- question ---
---
legend: 3లో 2వ ప్రశ్న
---

మౌస్ పాయింటర్ ను `touching`{:class="block3sensing"} `not`{:class="block3operators"} కండిషన్ ఉంటేనే తూనీగ కదిలేలా చేయడానికి మీరు కోడ్‌ని వ్రాసారు.

డ్రాగన్‌ఫ్లై కదిలిన ప్రతిసారీ ధ్వనిని ప్రారంభించేలా చేయడానికి మీరు `start sound`{:class="block3sound"} బ్లాక్‌ను ఎక్కడ ఉంచాలి?

--- choices ---

- ( )

```blocks3
when flag clicked
forever
+start sound [Wings v]
if <not <touching [mouse-pointer v] ?> > then
point towards (mouse-pointer v)
move [5] steps
end
end
```

--- feedback ---

లేదు, ఈ కోడ్‌తో `start sound`{:class="block3sound"} బ్లాక్ `if`{:class="block3control"} బ్లాక్‌కి వెలుపల ఉంది కాబట్టి, `forever`{:class="block3control"} లూప్ నడిచిన ప్రతిసారి, ఈ కోడ్ అమలు చేయబడుతుంది, తూనీగ కదలకపోయినా కూడా.

--- /feedback ---

- (x)

```blocks3
when flag clicked
forever
if <not <touching [mouse-pointer v] ?> > then
+start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

  --- feedback ---

అవును, అది సరైనది. `start sound`{:class="block3sound"} బ్లాక్‌ను `if`{:class="block3control"} బ్లాక్‌ లోపల ఉంచడం అంటే, తూనీగ కదిలినప్పుడు, అది ప్లే అవుతుంది.

  --- /feedback ---

- ( )


```blocks3
when flag clicked
forever
if <not <touching [mouse-pointer v] ?> > then
point towards (mouse-pointer v)
move [5] steps
end
+start sound [Wings v]
end
```

  --- feedback ---

లేదు, ఈ కోడ్‌తో `start sound`{:class="block3sound"} బ్లాక్ `if`{:class="block3control"} బ్లాక్‌కి వెలుపల ఉంది కాబట్టి, `forever`{:class="block3control"} లూప్ నడిచిన ప్రతిసారి, ఈ కోడ్ అమలు చేయబడుతుంది, తూనీగ కదలకపోయినా కూడా.

  --- /feedback ---

--- /choices ---

--- /question ---
