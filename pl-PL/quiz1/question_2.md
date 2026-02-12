
--- question ---
---
legend: Question 2 of 3
---

Napisałaś kod, aby ważka poruszała się tylko wtedy, gdy `nie`{:class="block3operators"} `dotyka`{:class="block3sensing"} wskaźnika myszy.

Gdzie umieścić blok `zagraj dźwięk`{:class="block3sound"}, aby ważka odtwarzała dźwięk za każdym razem, gdy się porusza?

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

Nie, z tym kodem blok `zagraj dźwięk`{:class="block3sound"} jest poza blokiem `jeżeli`{:class="block3control"}, więc będzie uruchamiany za każdym razem, gdy działa pętla `zawsze`{:class=" block3control"}, nawet jeśli ważka się nie porusza.

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

Tak, to jest poprawna odpowiedź. Umieszczenie bloku `zagraj dźwięk`{:class="block3sound"} wewnątrz bloku `jeżeli`{:class="block3control"} oznacza, że będzie on odtwarzany, gdy ważka się poruszy.

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

Nie, blok `zagraj dźwięk`{:class="block3sound"} jest poza blokiem `jeżeli`{:class="block3control"}, więc będzie uruchamiany za każdym razem, gdy działa pętla `zawsze`{:class=" block3control"}, nawet jeśli ważka się nie porusza.

  --- /feedback ---

--- /choices ---

--- /question ---
