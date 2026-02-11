## Snelle quiz

Beantwoord de drie vragen. Je wordt naar het juiste antwoord geleid.

Klik na het beantwoorden van elke vraag op **Controleer mijn antwoord**.

Veel plezier!

--- question ---
---
legend: Vraag 1 van 3
---

Een project maakt gebruik van de **Crab** (krab) sprite en de **Jellyfish** (kwal) sprite. De sprite **Crab** heeft deze code:

![desc](images/crab-icon.png)

```blocks3
when flag clicked
if <not <touching color (#0000FF)?>> then
hide
end
```

Wat moet er gebeuren om de sprite **Crab** te laten verdwijnen?

--- choices ---

- () De **Crab** sprite zou de **Jellyfish** moeten raken

 --- feedback ---

 Nee, het `als`{:class="block3control"}-blok heeft een `waarnemen`{:class="block3sensing"}-voorwaarde, maar het maakt geen gebruik van het `raak ik Jellyfish`{:class="block3sensing"}-blok.

 --- /feedback ---

- (x) De **Crab** sprite zou de kleur blauw niet moeten raken

 --- feedback ---

Ja, de `niet`{:class="block3operators"} operator betekent dat de voorwaarde waar is `als`{:class="block3control"} de **Crab** sprite niet de kleur blauw `aanraakt`{:class="block3sensing"}.

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
