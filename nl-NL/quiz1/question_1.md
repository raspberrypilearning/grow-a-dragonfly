## Quick quiz

Answer the three questions. There are hints to guide you to the correct answer.

When you have answered each question, click on **Check my answer**.

Have fun!

--- question ---
---
legend: Vraag 1 van 3
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

- () De **Crab** sprite zou de **Jellyfish** moeten raken

 --- feedback ---

 Nee, het `als`{:class="block3control"}-blok heeft een `waarnemen`{:class="block3sensing"}-voorwaarde, maar het maakt geen gebruik van het `raak ik Jellyfish`{:class="block3sensing"}-blok.

 --- /feedback ---

- (x) De **Crab** sprite zou de kleur blauw niet moeten raken

 --- feedback ---

Yes, the `not`{:class="block3operators"} operator means that the condition is true `if`{:class="block3control"} the **Crab** sprite is not `touching`{:class="block3sensing"} the colour blue.

 --- /feedback ---

- () De **Crab** sprite zou de kleur blauw moeten raken

 --- feedback ---

 Niet helemaal, kijk goed naar de `voorwaarde`{:class="block3operators"} in de functie.

 --- /feedback ---

- ( ) De **Crab** sprite zal altijd `verdwijnen`{:class="block3looks"} `wanneer op de groen vlag wordt geklikt`{:class="block3events"}

 --- feedback ---

 Nee, er is een `als`{:class="block3control"}-blok in de code van de **Crab** sprite, dus het wordt alleen verborgen als aan de voorwaarde wordt voldaan.

 --- /feedback ---

--- /choices ---

--- /question ---
