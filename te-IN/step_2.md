## సన్నివేశాన్ని సెట్ చేయండి

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
మీరు సన్నివేశాన్ని సెట్ చేస్తారు. మీ బ్యాక్‌డ్రాప్‌ను ఎంచుకుని, Stage చుట్టూ ఉన్న మౌస్ పాయింటర్‌ను అనుసరించే తూనీగని జోడించండి.
</div>
<div>
![](images/set-the-scene.png){:width="300px"}
</div>
</div>

--- task ---

[గ్రో ఎ డ్రాగన్‌ఫ్లై స్టార్టర్ ప్రాజెక్ట్](https://scratch.mit.edu/projects/535695413/editor){:target="_blank"}ని తెరవండి. Scratch మరొక బ్రౌజర్ ట్యాబ్‌లో తెరవబడుతుంది.

[[[working-offline]]]

--- /task ---

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">**తూనీగలను**</span> ప్రపంచవ్యాప్తంగా చూడవచ్చు మరియు 300 మిలియన్ సంవత్సరాలకు పైగా ఉన్నాయి!</p>

--- task ---

**ఎంచుకోండి:** **Choose a backdrop** మీద క్లిక్ చేయండి మరియు మీకు నచ్చిన బ్యాక్‌డ్రాప్‌ను జోడించండి. మనము **Jurassic** బ్యాక్‌డ్రాప్‌ని ఉపయోగించాము.

![](images/choose-backdrop-icon.png)

![జురాసిక్ బ్యాక్‌డ్రాప్‌ని చూపించే Stage.](images/Jurassic-backdrop.png)

--- /task ---

--- task ---

**Choose a sprite** మీద క్లిక్ చేయండి మరియు `dragonfly` అని శోధించండి, అటుపై **Dragonfly** sprite ను జోడించండి.

![](images/choose-sprite-icon.png)

![గ్యాలరీలో 'dragonfly' అని టైప్ చేసిన సెర్చ్ బాక్స్ మరియు Dragonfly sprite.](images/dragonfly-search.png)

--- /task ---

--- task ---

**Dragonfly** sprite మౌస్-పాయింటర్‌ను (లేదా మీ వేలు) అనుసరించేలా చేయడానికి స్క్రిప్ట్‌ను జోడించండి:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] % // చిన్నగా ప్రారంభించడానికి
forever
point towards (mouse-pointer v)
move [5] steps
end
```
--- /task ---

--- task ---

**పరీక్ష:** ఆకుపచ్చ జెండాపై క్లిక్ చేసి, **Dragonfly** sprite ను Stage చుట్టూ కదిలేలా చేయండి. మీరు అనుకున్నట్లుగా తూనీగ కదులుతుందా?

--- /task ---

తూనీగ costume కుడివైపున లేదు, కాబట్టి **Dragonfly** sprite యొక్క తల మౌస్-పాయింటర్ వైపు చూపడం లేదు.

--- task ---

**Costumes** ట్యాబ్‌పై క్లిక్ చేసి, **Select** (బాణం) సాధనాన్ని costume ఎంచుకోవడానికి ఉపయోగించండి. ఎంచుకున్న costume దిగువన గల **Rotate** సాధనాన్ని ఉపయోగించండి. మరియు **Dragonfly** costume ను కుడివైపుకు తిప్పడానికి ప్రయత్నించండి.

![తూనీగ కుడివైపుకు కనిపించేలా, రొటేషన్ బాణాలను లాగడం ద్వారా తూనీగ costume లను ఎలా తిప్పాలో చూపే యానిమేటెడ్ చిత్రం.](images/rotated-costume.gif)

![డ్రాగన్‌ఫ్లై costume ఎంచుకోబడింది మరియు కుడి వైపుకు తిరిగింది.](images/rotated-costume.png)

--- /task ---

--- task ---

**పరీక్ష:** ఆకుపచ్చ జెండాపై క్లిక్ చేసి, తూనీగ ఇప్పుడు ఎలా కదులుతుందో చూడండి.

--- /task ---

తూనీక రెక్కలు కంపిస్తున్నప్పుడు,. టపటపలాడిస్తున్న ధ్వనిని చేస్తున్నాయి. మీరు మీ స్వంత ధ్వనిని సృష్టించడానికి Scratch లో ధ్వనిని సవరించవచ్చు.

--- task ---

**Dragonfly** sprite **Crank** ధ్వనిని జోడించండి.

[[[generic-scratch3-sound-from-library]]]

![](images/crank-sound-editor.png)

**Play** బటన్‌ను క్లిక్ చేయండి, తద్వారా మీరు ధ్వనిని వినవచ్చు.

--- /task ---

**Crank** ధ్వని చాలా దీర్ఘంగా ఉంది మరియు తూనీగ రెక్కలకు చాలా నెమ్మదిగా ఉంది.

--- task ---

మీ కర్సర్ లేదా వేలిని ఉపయోగించి ధ్వని ముగింపును ఎంచుకోండి.

ఎంచుకున్న భాగంతో కొత్త ధ్వనిని చేయడానికి **Copy to New** ని క్లిక్ చేయండి:

![హైలైట్ చేయబడిన 'Copy to New ' ఐకాన్‌తో నీలం రంగులో ఎంచుకోబడిన క్రాంక్ సౌండ్ ముగింపు.](images/crank-copy-end.png)

మీ కొత్త ధ్వనిని **Crank2** నుండి `Wings`కి మార్చండి.

![ధ్వని లక్షణం పేరు మార్చండి.](images/crank-wings-sound.png)

--- /task ---

--- task ---

కొత్త ధ్వనిని ప్లే చేయండి. మీరు ఫలితాన్ని ఇష్టపడే వరకు **Faster** బటన్‌ను కొన్ని సార్లు క్లిక్ చేయండి:

!['Faster' చిహ్నం హైలైట్ చేయబడిన వేగవంతమైన ధ్వని తరంగం.](images/wings-faster.png)

--- /task ---

--- task ---

మీకు కావాలంటే, మీరు **Wings** సౌండ్ యొక్క ముగింపుని ఎంచుకోవచ్చు, ఆపై దాన్ని తీసివేయడానికి **Delete** మీద క్లిక్ చేయండి:

!['Delete' సాధనంతో ఎంపిక చేయబడిన ధ్వని తరంగం యొక్క ముగింపు హైలైట్ చేయబడింది.](images/wings-shorter.png)

--- /task ---

--- task ---

తూనీగ కదిలినప్పుడు **Wings** సౌండ్‌ని ప్లే చేయడానికి ఇప్పుడు ఒక బ్లాక్‌ని జోడించండి:

![](images/dragonfly-icon.png)

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

**పరీక్ష:** మీ డ్రాగన్‌ఫ్లై కదలిక మరియు ధ్వని ప్రభావాన్ని ప్రయత్నించండి.

--- /task ---

--- save ---
