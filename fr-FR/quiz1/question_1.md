## Réflexion

Bravo, tu as créé une application sur la nature avec une libellule contrôlée par l'utilisateur et des insectes qui suivent un algorithme !

Tu as utilisé les blocs `Événements`{:class="block3events"}, `Contrôle`{:class="block3control"}, `Capteurs`{:class="block3sensing"}, `Opérateurs`{:class="block3operators"}, `Mouvement`{:class="block3motion"}, `Apparence`{:class="block3looks"}, et `Son`{:class="block3sound"} !

Maintenant, il est temps de réfléchir - la réflexion est une partie importante de l'apprentissage, car elle aide à établir de nouvelles connexions dans ton cerveau.

Réponds aux trois questions ci-dessous pour réfléchir sur ce que tu as appris.

Après chaque question, appuie sur Soumettre. Tu seras guidé vers la bonne réponse. Tu peux faire cette activité autant de fois que tu le souhaites.

Amuse-toi bien !

--- question ---
---
legend : Question 1 sur 3
---

Un projet utilise le sprite **Crabe** et le sprite **Méduse**. Le sprite **Crabe** contient ce code :

![desc](images/crab-icon.png)

```blocks3
when flag clicked
if <not <touching color (#0000FF)?>> then
hide
end
```

Que devrait-il se passer pour que le sprite **Crabe** se cache ?

--- choices ---

- () Le sprite **Crabe** aurait besoin de toucher la **Méduse**

 --- feedback ---

 Non, le bloc `si`{:class="block3control"} a une condition `Capteurs`{:class="block3sensing"}, mais il n'utilise pas le bloc `touche la Méduse`{:class="block3sensing"}.

 --- /feedback ---

- (x) Le sprite **Crabe** ne devrait pas toucher la couleur bleue

 --- feedback ---

Oui, l'opérateur `non`{:class="block3operators"} signifie que la condition est vraie `si`{:class="block3control"} le sprite **Crabe** ne `touche`{:class="block3sensing"} pas la couleur bleue.

 --- /feedback ---

- () Le sprite **Crabe** devrait toucher la couleur bleue

 --- feedback ---

 Pas tout à fait, regarde attentivement l'`opérateur`{:class="block3operators"} dans la condition.

 --- /feedback ---

- ( ) Le sprite **Crabe** sera toujours `caché`{:class="block3looks"} `quand le drapeau vert est cliqué`{:class="block3events"}

 --- feedback ---

 Non, il y a un bloc `si`{:class="block3control"} dans le code du sprite **Crabe** donc il ne se cachera que si la condition est remplie.

 --- /feedback ---

--- /choices ---

--- /question ---
