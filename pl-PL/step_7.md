## Losowy ruch owada

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Owady w Twojej aplikacji poruszają się w bardzo przewidywalny sposób, ale w prawdziwym życiu trudno je złapać. 

Użyjesz bloku `losuj liczbę`{:class="block3operators"}, aby owad poruszał się w bardziej naturalny sposób.
</div>
<div>
![Scena pokazująca owady skierowane w różne strony.](images/random-movement.png){:width="300px"}
</div>
</div>

--- task ---

Dodaj skrypt do **Owad 2**, aby kierował się w losową stronę co 1–3 sekundy.

```blocks3
when flag clicked
forever // Keep changing direction
point in direction (pick random [0] to [259])
wait (pick random [1] to [3]) seconds
end
```

--- /task ---

--- task ---

**Test:** Uruchom swój projekt i obserwuj, jak porusza się mucha. Spróbuj zmienić liczby, aby uzyskać pożądany efekt.

Możesz również przeciągnąć ten skrypt do duszka **Owad**, aby również poruszał się losowo.

--- /task ---

--- task ---

Zmieniaj owady, aż będą zachowywać się tak, jak chcesz.

Możesz zmienić liczbę kroków, o które się `przesuwają`{:class="block3motion"}, aby były szybsze lub wolniejsze.

Możesz także zmienić prędkość ważki.

--- /task ---

--- task ---

Możesz także zmienić rozmiar, o który ważka musi urosnąć, aby osiągnąć pełny rozmiar.

Dokonuj zmian, aż będziesz zadowolony ze swojego projektu.

--- /task ---

--- save ---
