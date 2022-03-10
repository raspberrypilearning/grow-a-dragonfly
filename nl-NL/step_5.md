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

Sleep een `als`{:class="block3control"} blok binnen in het `herhaal`{:class="block3control"} blok en de blokken binnen het `herhaal`{:class="block3control"} blok zullen naar binnenin het `als`{:class="block3control"} blok verplaatsen.

Controleer zorgvuldig of je code er als volgt uitziet:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if < > then
start sound [Vleugels v]
point towards (mouse-pointer v)
move [5] steps
end
end
```
--- /task ---

--- task ---

Sleep vervolgens een `niet`{:class="block3operators"} blok naar het `als`{:class="block3control"} blok en een `raak ik (muiswijzer)`{:class="block3sensing"} blok daarin.

Kijk eerst of de code er zo uitziet:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if <not <touching [mouse-pointer v] ?> > then
start sound [Vleugels v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

Het `niet`{:class="block3operators"} blok verandert een voorwaarde in zijn tegenovergestelde, net zoals in een zin.

--- /task ---

--- task ---

**Test:** Controleer of de hapering is verholpen en dat de libel alleen beweegt als hij `niet`{:class="block3operators"} `de (muisaanwijzer) aanraakt`{:class="block3sensing"}.

Een andere voorwaarde om te proberen is:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

Dit zorgt ervoor dat de libel beweegt wanneer deze ver genoeg van de muisaanwijzer verwijderd is.

**Tip:** Je kunt blokken overal in het codegebied slepen en daar laten terwijl je verschillende dingen probeert.

--- /task ---

--- save ---
