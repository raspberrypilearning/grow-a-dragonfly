## మరింత ఆహారం

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
తూనీగకి కీటకాల ఎంపిక అవసరం.
</div>
<div>
![రెండు కీటకాలు మరియు తూనీగని చూపుతున్న Stage.](images/more-food.png){:width="300px"}
</div>
</div>

--- task ---

Sprite జాబితాలో **Insect** sprite పై రైట్-క్లిక్ చేసి, డ్రాప్-డౌన్ మెనులో **duplicate** ను సెలెక్ట్ చేసుకోండి.

![ఇన్సెక్ట్ sprite తో గల Sprite జాబితా ఎంపిక చేయబడింది మరియు మెనులో 'duplicate' హైలైట్ చేయబడింది.](images/duplicate-insect.png)

--- /task ---

ఈ కీటకం ఈగకి భిన్నంగా కనిపిస్తే అది ఉపయోగకరంగా ఉంటుంది.

--- task ---

**Costumes** ట్యాబ్‌పై క్లిక్ చేయండి.

వేరే ఎగిరే కీటకాన్ని సృష్టించడం ను**ఎంచుకోండి:**.
+ ఈ కీటకం రంగును మార్చడానికి **Fill** సాధనాన్ని ఉపయోగించండి
+ మీ స్వంత కీటకం costume లను **Paint** చేయండి
+ Scratch నుండి మరొక కీటకం costume లను **చేర్చండి**

--- /task ---

తూనీగ రెక్క లేదా తోకను తాకినా కూడా కీటకం తినబడుతుంది.

మీ యాప్‌ను మరింత వాస్తవికంగా చేయడానికి, తూనీగ నోటి ద్వారా కీటకాలను తినే విధంగా దీన్ని పరిష్కరించండి. మీరు `touching color`{:class="block3sensing"} బ్లాక్‌ని ఉపయోగించవచ్చు కాబట్టి **Dragonfly**పై నిర్దిష్ట రంగును తాకినట్లయితే మాత్రమే కీటకం తినబడుతుంది.

--- task ---

**Dragonfly** sprite ని ఎంచుకుని, **Costumes** ట్యాబ్‌పై క్లిక్ చేయండి.

**Dragonfly**నోటిని పూరించడానికి ఫిల్ సాధనాన్ని ఉపయోగించండి. మనము ఊదా రంగును ఉపయోగించాము:

![ఫిల్ టూల్‌తో పెయింట్ ఎడిటర్ ఎంపిక చేయబడింది మరియు ఊదా రంగు నోటితో తూనీగ costume.](images/dragonfly-mouth-colour.png)

--- /task ---

మీరు **Insect2** sprite **Dragonfly** sprite ను తాకుతున్నట్టు `మరియు (and)`{:class="block3operators"} తూనీగ నోటి రంగును తాకినట్లు తనిఖీ చేయాలి.

--- task ---

**Insect2** sprite ని ఎంచుకుని, **Code** ట్యాబ్‌పై క్లిక్ చేయండి.

`if`{:class="block3control"} బ్లాక్‌లో `and`{:class="block3operators"} బ్లాక్‌ని డ్రాగ్ చేయండి.

`<touching [Dragonfly v] ?>`{:class="block3sensing"} బ్లాక్ పాప్ అవుట్ అవుతుంది, దానిని `and`{:class="block3operators"} బ్లాక్‌కి ఎడమవైపుకి లాగండి:

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

`touching color`{:class="block3sensing"} బ్లాక్‌ని `and`{:class="block3operators"} బ్లాక్‌ యొక్క కుడివైపుకి లాగండి:

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

తూనీగ నోటి రంగు అందులో లేకపోతే, కలర్ సర్కిల్‌పై క్లిక్ చేసి, ఆపై రంగును ఎంచుకోవడానికి **Eyedropper** సాధనాన్ని ఉపయోగించండి.

![eyedropper సాధనంతో కలర్ సర్కిల్ మెను.](images/colour-eyedropper.png)

రంగును మ్యాచ్ అయ్యేలా సెట్ చేయడానికి Stage పై ఉన్న తూనీగ నోటిపై క్లిక్ చేయండి:

![కలర్ సెలెక్ట్ హైలైటర్‌ కల eyedropper సాధనం తూనీగ యొక్క ఊదారంగు నోటిపై తేలియాడుతుంది.](images/colour-select.png)

**చిట్కా:** దీన్ని చేయడం కష్టమైతే, **Dragonfly** sprite పరిమాణాన్ని, అది చాలా పెద్దదిగా అయ్యేలా మార్చండి,.

--- /task ---

--- task ---

**పరీక్ష:** ఇప్పుడు డ్రాగన్‌ఫ్లై తన నోటితో రెండవ కీటకాన్ని మాత్రమే తినగలదని పరీక్షించండి.

మీరు కావాలనుకుంటే, మొదటి **Insect** కాబట్టి అది కేవలం తూనీగ యొక్క నోటి ద్వారా మాత్రమే తినబడుతుంది.

--- /task ---

--- save ---

