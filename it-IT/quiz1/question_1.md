## Quiz veloce

Rispondi alle tre domande. Alcuni suggerimenti ti aiuteranno a trovare la risposta corretta.

Dopo aver risposto a ciascuna domanda, fai clic su **Controlla la mia risposta**.

Divertiti!

--- question ---
---
legend: Domanda 1 di 3
---

Un progetto utilizza lo sprite **Granchio** e lo sprite **Medusa**. Lo sprite **Granchio** ha questo codice:

![](images/crab-icon.png)

```blocks3
when flag clicked
if <not <touching color (#0000FF)?>> then
hide
end
```

Cosa dovrebbe succedere perché lo sprite **Granchio** si nasconda?

--- choices ---

- () Lo sprite **Granchio** dovrebbe toccare le **Meduse**

 --- feedback ---

 No, il blocco `se`{:class="block3control"} ha una condizione `Sensori`{:class="block3sensing"}, ma non usa il blocco `sta toccando Medusa`{:class="block3sensing"}.

 --- /feedback ---

- (x) Lo sprite **Granchio** non dovrebbe toccare il colore blu

 --- feedback ---

Si, l'operatore `non`{:class="block3operators"} significa che la condizione è vera `se`{:class="block3control"} lo sprite **Granchio** non `sta toccando`{:class="block3sensing"} il colore blu.

 --- /feedback ---

- () Lo sprite **Granchio** dovrebbe toccare il colore blu

 --- feedback ---

 Non proprio, guarda attentamente gli `operatori`{:class="block3operators"} nella condizione.

 --- /feedback ---

- ( ) Lo sprite **Granchio** lo `nascondi`{:class="block3looks"} sempre `quando la bandiera viene cliccata`{:class="block3events"}

 --- feedback ---

 No, c'è un blocco `se`{:class="block3control"} nel codice dello sprite **Granchio** quindi verrà nascosto solo se la condizione è soddisfatta.

 --- /feedback ---

--- /choices ---

--- /question ---
