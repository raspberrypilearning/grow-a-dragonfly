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

Drag an `if`{:class="block3control"} inside the `forever`{:class="block3control"} block. The blocks inside the `forever`{:class="block3control"} will move inside the `if`{:class="block3control"}.

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

Then drag a `not`{:class="block3operators"} block into the `if`{:class="block3control"} and a `touching (mouse-pointer)`{:class="block3sensing"} inside that.

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

--- /task ---

--- task ---

**పరీక్ష:** గ్లిచ్ పరిష్కరించబడిందో లేదో తనిఖీ చేయండి మరియు Dragonfly `touching (mouse-pointer`{:class="block3sensing"} లేనప్పుడు ` not`{:class="block3operators"} మాత్రమే కదులుతుంది.

--- /task ---

--- task ---

Try a different condition that makes the dragonfly move when it is far enough from the mouse-pointer:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

--- /task ---

--- save ---
