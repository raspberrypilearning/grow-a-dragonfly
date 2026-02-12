## Questionnaire rapide

Réponds aux trois questions. Il y a des indices pour te guider vers la bonne réponse.

Lorsque tu as répondu à chaque question, clique sur **Vérifier ma réponse**.

Amuse-toi bien !

--- question ---
---
legend: Question 1 sur 3
---

Un projet utilise le sprite **Crab** (Crabe) et le sprite **Jellyfish** (Méduse). Le sprite **Crabe** contient ce code :

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
