## Mouvement amélioré

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
La libellule « glisse » et change de direction très rapidement si le pointeur de la souris touche la libellule. Tu vas vérifier une autre condition pour résoudre ce problème.
</div>
<div>
![La scène montrant un insecte et une libellule.](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

Sélectionne la **Libellule** et trouve le script qui commence par `Quand le drapeau vert est cliqué`{:class="block3events"}.

Fais glisser un `si`{:class="block3control"} à l'intérieur du bloc `répéter indéfiniment`{:class="block3control"} et les blocs à l'intérieur du `répéter indéfiniment`{:class="block3control"} se déplaceront à l'intérieur du `si`{:class="block3control"}. The blocks inside the `forever`{:class="block3control"} will move inside the `if`{:class="block3control"}.

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

Ensuite, fais glisser un bloc `non`{:class="block3operators"} dans le `si`{:class="block3control"} et un `touche le (pointeur de la souris)`{:class="block3sensing"} à l'intérieur.

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

**Test :** Vérifie que le problème est résolu et que la libellule ne bouge que lorsque `non`{:class="block3operators"} `touche le (pointeur de la souris)`{:class="block3sensing"}.

--- /task ---

--- task ---

Try a different condition that makes the dragonfly move when it is far enough from the mouse-pointer:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

--- /task ---

--- save ---
