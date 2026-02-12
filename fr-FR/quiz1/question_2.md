
--- question ---
---
legend: Question 2 sur 3
---

Tu as écrit du code pour faire bouger la libellule uniquement si `non`{:class="block3operators"} `touche`{:class="block3sensing"} le pointeur de la souris.

Où placerais-tu un bloc `jouer le son`{:class="block3sound"} pour que la libellule émette un son à chaque fois qu'elle bouge ?

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

Non, avec ce code, le bloc `jouer le son`{:class="block3sound"} est en dehors du bloc `si`{:class="block3control"}, il s'exécutera donc à chaque fois que la boucle `répéter indéfiniment`{:class="block3control"} s'exécute, même si la libellule ne bouge pas.

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

Oui c'est correct. Placer le bloc `jouer le son`{:class="block3sound"} à l'intérieur du bloc `si`{:class="block3control"} signifie qu'il jouera lorsque la libellule se déplacera.

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

Non, le bloc `jouer le son`{:class="block3sound"} est en dehors du bloc `si`{:class="block3control"}, il s'exécutera donc à chaque fois que la boucle `répéter indéfiniment`{:class="block3control"} fonctionne, même si la libellule ne bouge pas.

  --- /feedback ---

--- /choices ---

--- /question ---
