## Migliora il movimento

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
La libellula "si blocca" e cambia direzione molto velocemente se il puntatore del mouse tocca la libellula. Inserirai un'altra condizione per risolvere questo problema.
</div>
<div>
![Lo Stage con un insetto e una libellula.](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

Seleziona la **libellula** e trova lo script che inizia con `quando si fa clic su bandierina verde`{:class="block3events"}.

Trascina un blocco `se`{:class="block3control"} dentro il blocco `per sempre`{:class="block3control"} e i blocchi dentro `per sempre`{:class="block3control"} si sposteranno dentro il blocco `se`{:class="block3control"}.

Controlla attentamente che il tuo codice assomigli a questo:

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

Poi trascina un blocco `non`{:class="block3operators"} dentro `se`{:class="block3control"} e un `sta toccando (puntatore del mouse)`{:class="block3sensing"}.

Controlla che il tuo codice sia simile a questo:

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

Il blocco `non`{:class="block3operators"} trasforma una condizione nel suo opposto, proprio come farebbe in una frase.

--- /task ---

--- task ---

**Test:** Controlla che il blocco non si verifichi, e la libellula si muova solo quando `non`{:class="block3operators"} `sta toccando (puntatore del mouse)`{:class="block3sensing"}.

Una condizione diversa da provare è:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

Questo fa muovere la libellula quando è abbastanza lontana dal puntatore del mouse.

**Suggerimento:** Puoi trascinare i blocchi ovunque nell'area Codice e lasciarli lì mentre provi soluzioni diverse.

--- /task ---

--- save ---
