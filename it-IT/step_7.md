## Movimento casuale degli insetti

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Gli insetti nella tua app si muovono secondo uno schema molto prevedibile, ma nella vita reale sono difficili da catturare. 

Utilizzerai il blocco `numero a caso`{:class="block3operators"} per far muovere l'insetto in un modo più naturale.
</div>
<div>
![Stage che mostra insetti che puntano in direzioni diverse.](images/random-movement.png){:width="300px"}
</div>
</div>

--- task ---

Aggiungi uno script a **insetto2** per farlo puntare in una direzione casuale ogni 1-3 secondi.

```blocks3
when flag clicked
forever // Continua a cambiare direzione
point in direction (pick random [0] to [259])
wait (pick random [1] to [3]) seconds
end
```

--- /task ---

--- task ---

**Test:** Esegui il tuo progetto e osserva come si muove la mosca. Prova a cambiare i numeri per ottenere l'effetto desiderato.

Puoi anche trascinare questo script sullo sprite **insetto** in modo che anche lui si muova in modo casuale.

--- /task ---

--- task ---

Cambia gli insetti finché non si comportano come desideri.

Puoi modificare il numero di passi in `movimento`{:class="block3motion"} per renderli più veloci o più lenti.

Potresti anche cambiare la velocità della libellula.

--- /task ---

--- task ---

Potresti anche modificare le dimensioni che la libellula deve ottenere per raggiungere la dimensione massima.

Apporta modifiche finché non sei soddisfatto del tuo progetto.

--- /task ---

--- save ---
