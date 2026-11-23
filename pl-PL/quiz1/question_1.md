## Szybki quiz

Odpowiedz na trzy pytania. Podpowiedzi naprowadzą Cię na właściwą odpowiedź.

Po udzieleniu odpowiedzi na każde pytanie kliknij przycisk **Sprawdź moją odpowiedź**.

Miłej zabawy!

--- question ---
---
legend: Question 1 of 3
---

Projekt używa duszka **Krab** (ang. Crab) i duszka **Meduza** (ang. Jellyfish). Duszek **Krab** ma następujący kod:

![opis](images/crab-icon.png)

```blocks3
when flag clicked
if <not <touching color (#0000FF)?>> then
hide
end
```

Kiedy duszek **Krab** się ukryje?

--- choices ---

- () Duszek **Krab** dotknie **Meduzy**

 --- feedback ---

 Nie, blok `Jeżeli`{:class="block3control"} ma warunek `dotyka`{:class="block3sensing"}, ale nie używa bloku `dotykania Meduza`{:class="block3sensing"}.

 --- /feedback ---

- (x) Duszek **Krab** nie dotnie koloru niebieskiego

 --- feedback ---

Tak, `nie` {:class="block3operators"} oznacza, że warunek jest prawdziwy `jeśli` {:class="block3control"} **Krab nie **dotyka`` {:class="block3sensing"} koloru niebieskiego.

 --- /feedback ---

- (x) Duszek **Krab** dotknie koloru niebieskiego

 --- feedback ---

 Niezupełnie, spójrz uważnie na `operator`{:class="block3operators"} w warunku.

 --- /feedback ---

- ( ) Duszek **Krab** zawsze się`ukryje`{:class="block3looks"} `kiedy kliknięto flagę`{:class="block3events"}

 --- feedback ---

 Nie, blok `jeżeli`{:class="block3control"} jest w kodzie duszka **Krab**, więc ukryje się tylko, jeśli warunek zostanie spełniony.

 --- /feedback ---

--- /choices ---

--- /question ---
