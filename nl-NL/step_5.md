## Verbeterde beweging

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
De libel 'hapert' en verandert heel snel van richting als de muisaanwijzer de libel aanraakt. Je gaat een andere voorwaarde proberen om dit op te lossen.
</div>
<div>
![Het speelveld toont een insect en een libel.](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

Selecteer de **libel** en zoek het script dat begint met `wanneer op de vlag wordt geklikt`{:class="block3events"}.

Sleep een `als`{:class="block3control"} blok binnen in het `herhaal`{:class="block3control"} blok en de blokken binnen het <0>herhaal</0>{:class="block3control"} blok zullen naar het <0>als</0>{:class="block3control"} blok worden verplaatst. De blokken in het `herhaal`{:class="block3control"} blok worden verplaatst naar het `als`{:class="block3control"} blok.

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

Sleep vervolgens een `niet`{:class="block3operators"} blok naar het `als`{:class="block3control"} blok en een `raak ik (muisaanwijzer)`{:class="block3sensing"} blok daarin.

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

**Test:** Controleer of de hapering is verholpen en dat de libel alleen beweegt als hij `niet`{:class="block3operators"} `de (muisaanwijzer) aanraakt`{:class="block3sensing"}.

--- /task ---

--- task ---

Probeer een andere voorwaarde waardoor de libel beweegt als hij ver genoeg van de muisaanwijzer verwijderd is:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

--- /task ---

--- save ---
