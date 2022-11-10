## Quick quiz

Answer the three questions. There are hints to guide you to the correct answer.

When you have answered each question, click on **Check my answer**.

Have fun!

--- question ---
---
legend : Question 1 sur 3
---

A project uses the **Crab** sprite and the **Jellyfish** sprite. The **Crab** sprite has this code:

![desc](images/crab-icon.png)

```blocks3
when flag clicked
if <not <touching color (#0000FF)?>> then
hide
end
```

What would need to happen for the **Crab** sprite to hide?

--- choices ---

- () Le sprite **Crabe** aurait besoin de toucher la **Méduse**

 --- feedback ---

 Non, le bloc `si`{:class="block3control"} a une condition `Capteurs`{:class="block3sensing"}, mais il n'utilise pas le bloc `touche la Méduse`{:class="block3sensing"}.

 --- /feedback ---

- (x) Le sprite **Crabe** ne devrait pas toucher la couleur bleue

 --- feedback ---

Yes, the `not`{:class="block3operators"} operator means that the condition is true `if`{:class="block3control"} the **Crab** sprite is not `touching`{:class="block3sensing"} the colour blue.

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
