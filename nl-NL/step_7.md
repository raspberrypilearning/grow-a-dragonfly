## Uitdaging

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Verander het gedrag van je insecten en voeg meer insecten toe.
</div>
<div>
![Het speelveld toont drie verschillende soorten insecten en de libel.](images/upgrade-project.png){:width="300px"}
</div>
</div>

--- task ---

Verander de snelheid van de libel.

--- /task ---

--- task ---

Je kunt ook de grootte wijzigen die de libel nodig heeft om te groeien om de volledige grootte te bereiken.

--- /task ---

--- task ---

Verander het eerste **insect** zodat het alleen met de mond van de libel gegeten kan worden.

--- /task ---

### Voeg meer insecten toe

Je kunt je eigen insecten tekenen of proberen een emoji-mug toe te voegen!

--- task ---

Gebruik het emoji-toetsenbord om een **mug-emoji** sprite toe te voegen.

Dupliceer een bestaande **insecten** sprite en klik vervolgens op het tabblad **Uiterlijken**. **Teken** een nieuw uiterlijk en selecteer het gereedschap **Tekst**. Gebruik in plaats van tekst te typen de emoji-sneltoets van je besturingssysteem:

- Windows - <kbd>⊞ Win</kbd> + <kbd>.</kbd>
- MacOS - <kbd>control</kbd> + <kbd>command</kbd> + <kbd>space</kbd>
- Linux - <kbd>ctrl</kbd> + <kbd>.</kbd>

![Het pop-up venster met het emoji-toetsenbord met de categorie 'dieren en natuur' geselecteerd.](images/emoji-keyboard.png)

Selecteer de **Mug** emoji om deze in de Paint-editor in te voegen. Gebruik het gereedschap **Selecteren** (pijl) om je mug te centreren, vergroten of verkleinen en roteren totdat je er tevreden mee bent.

![De mug-emoji in de tekeneditor.](images/emoji-mosquito.png)

**Tip:** Emoji's kunnen er op verschillende computers anders uitzien, dus ze zien er mogelijk niet hetzelfde uit op een tablet en een desktopcomputer. Sommige emoji's zijn niet beschikbaar op sommige computers, maar de meeste moderne computers zullen ze wel ondersteunen.

--- /task ---

### Creëer willekeurige beweging

Je gebruikt het `willekeurig getal tussen`{:class="block3operators"} blok om het insect op een meer natuurlijke manier te laten bewegen.

![Een speelveld waarop insecten in verschillende richtingen wijzen.](images/random-movement.png){:width="300px"}

--- task ---

Voeg een script toe aan **Insect 2** zodat het elke 1 tot 3 seconden in een willekeurige richting wijst.

![](images/insect2-icon.png)

```blocks3
when flag clicked
forever // Keep changing direction
point in direction (pick random [0] to [259])
wait (pick random [1] to [3]) seconds
end
```

--- /task ---

--- task ---

**Test:** Test je project en bekijk hoe de insecten vliegen.

--- /task ---

--- task ---

Je kunt dit script ook naar de sprite **Insect** slepen, zodat het ook willekeurig beweegt.

--- /task ---

### Deel je insecten

--- task ---

Gebruik je rugzak om insecten te ruilen met je vrienden uit hun 'Laat een libel groeien'-projecten.

Stuur de link van je project naar een vriend(in) die het project kan openen, op Rugzak (het item onder de code) kan klikken en de sprite daarheen kan slepen.

[[[scratch-backpack]]]

--- /task ---

--- task ---

Controleer of elke sprite en uiterlijk een naam heeft die de afbeelding beschrijft. Hierdoor is je project gemakkelijker te begrijpen als je er later op terugkomt.

--- /task ---

--- task ---

Klik met de rechtermuisknop op het codegebied en kies **Blokken opruimen** om Scratch je code te laten opschonen.

--- /task ---

--- save ---
