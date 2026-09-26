
--- question ---
---
legend: Vraag 2 van 3
---

Je hebt code geschreven om de libel alleen te laten bewegen als deze `niet`{:class="block3operators"} de muisaanwijzer `aanraakt`{:class="block3sensing"}.

Waar zou je een `start geluid`{:class="block3sound"}-blok plaatsen om de libel een geluid te laten starten elke keer dat hij beweegt?

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

Nee, met deze code bevindt het `start geluid`{:class="block3sound"}-blok zich buiten het `als`{:class="block3control"}-blok, dus het wordt elke keer uitgevoerd als de `herhaal`{:class=" block3control"} lus loopt, zelfs als de libel niet beweegt.

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

Ja dat is goed. Het plaatsen van het `start geluid`{:class="block3sound"} blok binnen het `als`{:class="block3control"} blok betekent dat het zal spelen wanneer de libel beweegt.

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

Nee, met deze code bevindt het `start geluid`{:class="block3sound"}-blok zich buiten het `als`{:class="block3control"}-blok, dus het wordt elke keer uitgevoerd als de `herhaal`{:class=" block3control"} lus loopt, zelfs als de libel niet beweegt.

  --- /feedback ---

--- /choices ---

--- /question ---
