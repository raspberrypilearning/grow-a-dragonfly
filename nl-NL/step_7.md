## Willekeurige beweging van insecten

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
De insecten in je app bewegen in een zeer voorspelbaar patroon, maar in het echte leven zijn ze moeilijk te vangen. 

Je gebruikt het `willekeurig getal tussen`{:class="block3operators"} blok om het insect op een meer natuurlijke manier te laten bewegen.
</div>
<div>
![Speelveldmet insecten die in verschillende richtingen wijzen.](images/random-movement.png){:width="300px"}
</div>
</div>

--- task ---

Voeg een script toe aan **Insect 2** zodat het elke 1 tot 3 seconden in een willekeurige richting wijst.

```blocks3
when flag clicked
forever // Blijf van richting veranderen
point in direction (pick random [0] to [259])
wait (pick random [1] to [3]) seconds
end
```

--- /task ---

--- task ---

**Test:** Test je project en bekijk hoe de insecten vliegen. Probeer de getallen te veranderen om het gewenste effect te krijgen.

Je kunt dit script ook naar de sprite **Insect** slepen, zodat het ook willekeurig beweegt.

--- /task ---

--- task ---

Verander de insecten totdat ze zich gedragen zoals jij dat wilt.

Je kunt het aantal stappen dat ze `verplaatsen`{:class="block3motion"} wijzigen om ze sneller of langzamer te maken.

Je kunt ook de snelheid van de libel veranderen.

--- /task ---

--- task ---

Je kunt ook de grootte wijzigen die de libel nodig heeft om te groeien om de volledige grootte te bereiken.

Breng wijzigingen aan totdat je tevreden bent met jouw project.

--- /task ---

--- save ---
