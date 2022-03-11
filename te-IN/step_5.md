## మెరుగైన కదలిక

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
మౌస్-పాయింటర్ తూనీగని తాకినట్లయితే తూనీగ 'గ్లిచ్' అవుతుంది మరియు దిశను చాలా వేగంగా మారుస్తుంది. దీన్ని పరిష్కరించడానికి మీరు మరొక కండిషన్ ను తనిఖీ చేస్తారు.
</div>
<div>
![ఒక కీటకం మరియు తూనీగని చూపుతున్న Stage.](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

**Dragonfly**ని ఎంచుకోండి మరియు `when flag clicked`{:class="block3events"} తో మొదలయ్యే స్క్రిప్ట్‌ను కనుగొనండి.

`if`{:class="block3control"} బ్లాక్ ని `forever`{:class="block3control"} బ్లాక్ లోపలికి డ్రాగ్ చేయండి మరియు `forever`{:class="block3control"} లోపలనున్న బ్లాక్స్ `if`{:class="block3control"} లోపలికి చేరుకొంటాయి.

మీ కోడ్ ఇలా ఉందో లేదో జాగ్రత్తగా తనిఖీ చేయండి:

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

ఆపై `not`{:class="block3operators"} బ్లాక్‌ని `if`{:class="block3control"} లోకి మరియు `touching (mouse-pointer)`{:class="block3sensing"} ని డ్రాగ్ చేయండి.

మీ కోడ్ ఇలా ఉందో లేదో తనిఖీ చేయండి:

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

`not`{:class="block3operators"} బ్లాక్ ఒక కండిషన్ ను దాని వ్యతిరేక స్థితిగా మారుస్తుంది, అది వాక్య ప్రయోగంలో వాడకం వలే.

--- /task ---

--- task ---

**పరీక్ష:** గ్లిచ్ పరిష్కరించబడిందో లేదో తనిఖీ చేయండి మరియు Dragonfly `touching (mouse-pointer)`{:class="block3sensing"} లేనప్పుడు `not`{:class="block3operators"} మాత్రమే కదులుతుంది.

ప్రయత్నించడానికి వేరొక కండిషన్:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

ఇది మౌస్-పాయింటర్ నుండి తగినంత దూరంలో ఉన్నప్పుడు తూనీగ కదిలేలా చేస్తుంది.

**చిట్కా:** మీరు కోడ్ ప్రాంతంలో ఎక్కడైనా బ్లాక్‌లను లాగవచ్చు మరియు మీరు వివిధ విషయాలను ప్రయత్నించినప్పుడు వాటిని అక్కడ వదిలివేయవచ్చు.

--- /task ---

--- save ---
