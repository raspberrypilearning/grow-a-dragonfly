## Prepara la scena

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Preparerai la scena. Scegli lo sfondo e aggiungi una libellula che segue il puntatore del mouse sullo sfondo.
</div>
<div>
![Libellula con sfondo del deserto](images/set-the-scene.png){:width="300px"}
</div>
</div>

--- task ---

Apri il progetto [Alleva una libellula](https://scratch.mit.edu/projects/535695413/editor){:target="_blank"}. Scratch si aprirà in una nuova scheda del browser.

[[[working-offline]]]

--- /task ---

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">**Le libellule**</span> si trovano in tutto il mondo e esistono da oltre 300 milioni di anni!</p>

--- task ---

**Scegli:** Fai clic su **Scegli uno sfondo** e aggiungi uno sfondo a tua scelta. Abbiamo utilizzato lo sfondo **Giurassico**.

![Icona dello sfondo sull'interfaccia dell'app Scratch](images/choose-backdrop-icon.png)

![L'area mostra lo sfondo giurassico.](images/Jurassic-backdrop.png)

--- /task ---

--- task ---

Fai clic su **Scegli uno sprite** e cerca `dragonfly (libellula)`, quindi aggiungi lo sprite **libellula**.

![L'icona Sprite sull'interfaccia dell'app Scratch](images/choose-sprite-icon.png)

![La casella di ricerca con "dragonfly" digitata e lo sprite della libellula nella galleria.](images/dragonfly-search.png)

--- /task ---

--- task ---

Aggiungi del codice per fare in modo che lo sprite **Libellula** segua il puntatore del mouse (o il tuo dito):

![Icona dello sprite della libellula sull'interfaccia dell'app Scratch](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] % // dimensione iniziale piccola
forever
point towards (puntatore del mouse v)
move [5] steps
end
```
--- /task ---

--- task ---

**Test:** Clicca sulla bandiera verde e fai muovere lo sprite **libellula** sul palco. La libellula si muove come ti aspetteresti?

--- /task ---

Il costume della Libellula non è rivolto a destra, quindi la testa dello sprite **libellula** non punta verso il puntatore del mouse.

--- task ---

Clicca sulla scheda **Costumi** e usa lo strumento **Seleziona** (freccia) per selezionare il costume. Usa lo strumento **Ruota** nella parte inferiore del costume selezionato per girare la **libellula** verso destra.

![Un'immagine animata che mostra come ruotare il costume della libellula trascinando le frecce di rotazione in modo che la libellula sia rivolta verso destra.](images/rotated-costume.gif)

![Il costume da libellula selezionato e ruotato verso destra.](images/rotated-costume.png)

--- /task ---

--- task ---

**Test:** Clicca sulla bandiera verde e guarda come si muove ora la libellula.

--- /task ---

Le ali della libellula emettono un suono mentre vibrano. Puoi modificare un suono in Scratch per creare il tuo suono.

--- task ---

Aggiungi il suono **Crank** allo sprite **libellula**.

[[[generic-scratch3-sound-from-library]]]

![](images/crank-sound-editor.png)

Fai clic sul pulsante **Riproduci** per poter ascoltare il suono.

--- /task ---

Il suono **Crank** è troppo lungo e troppo lento per le ali della libellula.

--- task ---

Seleziona la fine del suono utilizzando il cursore o il dito.

Fai clic su **Copialo come nuovo suono** per creare un nuovo suono solo con la parte selezionata:

![La fine del suono Crank selezionato in blu con l'icona "Copialo come nuovo suono" evidenziata.](images/crank-copy-end.png)

Rinomina il tuo nuovo suono da **Crank2** ad `Ali`.

![Rinominare le proprietà del suono.](images/crank-wings-sound.png)

--- /task ---

--- task ---

Riproduci il nuovo suono. Fai clic sul pulsante **Accelera** alcune volte finché non ti piace il risultato:

![Un'onda sonora più veloce con l'icona "Accelera" evidenziata.](images/wings-faster.png)

--- /task ---

--- task ---

Se lo desideri, puoi selezionare la fine del suono di **Ali**, quindi fare clic su **Elimina** per rimuoverlo:

![La fine dell'onda sonora selezionata con lo strumento "Elimina" evidenziato.](images/wings-shorter.png)

--- /task ---

--- task ---

Ora aggiungi un blocco per riprodurre il suono delle **Ali** quando la libellula si muove:

![Icona dello sprite della libellula](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+start sound [Wings v]
point towards (puntatore del mouse v)
move [5] steps
end
```
--- /task ---

--- task ---

**Test:** Prova il movimento della libellula e l'effetto sonoro.

--- /task ---

--- save ---
