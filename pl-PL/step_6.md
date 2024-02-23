## Więcej pokarmu

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Ważka potrzebuje dokonać wyboru owada.
</div>
<div>
![Scena z dwoma owadami i ważką.](images/more-food.png){:width="300px"}
</div>
</div>

--- task ---

Kliknij prawym przyciskiem myszy duszka **Owad** na liście duszków pod sceną i wybierz **duplikuj**.

![Lista duszków z wybranym duszkiem owada i zaznaczonym „duplikuj” w menu.](images/duplicate-insect.png)

--- /task ---

Dobrze, jeśli ten owad wygląda inaczej niż mucha.

--- task ---

Naciśnij na zakładkę **Kostiumy**.

**Wybierz:** Utwórz innego latającego owada.
+ Użyj narzędzia **Wypełnij**, aby zmienić kolor owada
+ **Pomaluj** stworzony przez siebie kostium owada
+ **Dodaj** kolejny kostium robaka ze Scratcha

--- /task ---

Owad zostaje zjedzony, nawet jeśli dotknie skrzydła lub ogona ważki.

Aby Twoja aplikacja była bardziej realistyczna, popraw to, by owad był zjadany tylko po dotknięciu buzi ważki. Możesz użyć bloku `dotyka koloru`{:class="block3sensing"}, aby owad został zjedzony tylko wtedy, gdy dotknie określonego koloru na **Ważce**.

--- task ---

Wybierz duszka **Ważka** i kliknij zakładkę **Kostiumy**.

Użyj narzędzia do wypełniania, aby wypełnić buzię **Ważki**. My użyliśmy fioletu:

![Edytor malowania z wybranym narzędziem Wypełnienie i kostiumem ważki z fioletową buzią.](images/dragonfly-mouth-colour.png)

--- /task ---

Musisz sprawdzić, czy duszek **Owad2** dotyka duszka **Ważka** `i`{:class="block3operators"} dotyka koloru buzi ważki.

--- task ---

Wybierz duszka **Owad2** i kliknij zakładkę **Skrypt**.

Przeciągnij blok `i`{:class="block3operators"} do wnętrza bloku `jeżeli`{:class="block3control"}.

Kiedy wyskoczy blok `<touching [Dragonfly v] ?>`{:class="block3sensing"}, przeciągnij go na lewo od bloku `i`{:class="block3operators"}:

![](images/insect2-icon.png)

```blocks3
when flag clicked
show
forever
move [3] steps 
if on edge, bounce
+if <<touching [Dragonfly v] ?> and <>> then
broadcast [food v]
hide
go to (random position v)
show
end
end
```

--- /task ---

--- task ---

Przeciągnij blok `dotyka koloru`{:class="block3sensing"} na prawo od bloku `i`{:class="block3operators"}:

![](images/insect2-icon.png)

```blocks3
when flag clicked
show
forever
move [3] steps
if on edge, bounce
+if <<touching [Dragonfly v] ?> and <touching color (#9966ff) ?>> then
broadcast [food v]
hide
go to (random position v)
show
end
end
```

Jeśli nie ma wybranego koloru buzi ważki, kliknij na koło wyboru kolorów, a następnie kliknij narzędzie **Kroplomierz**, aby wybrać kolor.

![Menu koła kolorów z narzędziem kroplomierza.](images/colour-eyedropper.png)

Kliknij znajdującą się na Scenie buzię ważki, aby ustawić odpowiedni kolor:

![Kroplomierz z zakreślaczem do wyboru koloru znajdującym się nad fioletową buzią ważki.](images/colour-select.png)

**Wskazówka:** Jeśli jest to trudne do zrobienia, zmień rozmiar duszka **Ważka** tak, aby był naprawdę duży.

--- /task ---

--- task ---

**Test:** Teraz sprawdź, czy ważka może zjeść drugiego owada tylko buzią.

Jeśli chcesz, możesz zmienić pierwszego duszka **Owad** tak, aby można było go zjeść tylko buzią ważki.

--- /task ---

--- save ---

