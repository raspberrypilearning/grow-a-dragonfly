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

Fais glisser un `si`{:class="block3control"} à l'intérieur du bloc `répéter indéfiniment`{:class="block3control"} et les blocs à l'intérieur du `répéter indéfiniment`{:class="block3control"} se déplaceront à l'intérieur du `si`{:class="block3control"}.

Vérifie bien que ton code ressemble à ceci :

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

Vérifie bien que ton code ressemble à ceci :

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

Le bloc `non`{:class="block3operators"} transforme une condition en son contraire, comme il le ferait dans une phrase.

--- /task ---

--- task ---

**Test :** Vérifie que le problème est résolu et que la libellule ne bouge que lorsque `non`{:class="block3operators"} `touche le (pointeur de la souris)`{:class="block3sensing"}.

Une condition différente à essayer est :

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

Cela fait bouger la libellule lorsqu'elle est suffisamment éloignée du pointeur de la souris.

**Astuce :** Tu peux faire glisser des blocs n'importe où dans la zone de code et les y laisser pendant que tu essaies différentes choses.

--- /task ---

--- save ---
