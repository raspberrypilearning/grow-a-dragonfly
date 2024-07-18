
--- question ---
---
legend: Domanda 2 di 3
---

Hai scritto il codice per far muovere la libellula solo se `non`{:class="block3operators"} `sta toccando`{:class="block3sensing"} il puntatore del mouse.

Dove inseriresti un blocco `avvia riproduzione suono`{:class="block3sound"} per far sì che la libellula emetta un suono ogni volta che si muove?

--- choices ---

- ( )

```blocks3
when flag clicked
forever
+start sound [Wings v]
if <not <touching [mouse-pointer v] ?> > then
point towards (mouse-pointer v)
move [5] steps
end
end
```

--- feedback ---

No, con questo codice il blocco `avvia riproduzione suono`{:class="block3sound"} è esterno al blocco `se`{:class="block3control"}, quindi verrà eseguito ogni volta che viene eseguito il ciclo `per sempre`{:class="block3control"}, anche se la libellula non si muove.

--- /feedback ---

- (x)

```blocks3
when flag clicked
forever
if <not <touching [mouse-pointer v] ?> > then
+start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

  --- feedback ---

Sì, è corretto. Posizionando il blocco `avvia riproduzione suono`{:class="block3sound"} all'interno del blocco `se`{:class="block3control"} significa che verrà riprodotto quando la libellula si muove.

  --- /feedback ---

- ( )


```blocks3
when flag clicked
forever
if <not <touching [mouse-pointer v] ?> > then
point towards (mouse-pointer v)
move [5] steps
end
+start sound [Wings v]
end
```

  --- feedback ---

No, il blocco `avvia riproduzione suono`{:class="block3sound"} è esterno al blocco `se`{:class="block3control"}, quindi verrà eseguito ogni volta che viene eseguito il ciclo `per sempre`{:class="block3control"}, anche se la libellula non si muove.

  --- /feedback ---

--- /choices ---

--- /question ---
