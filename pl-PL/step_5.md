## Poprawiony ruch

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Ważka ma 'usterkę' i zmienia kierunek bardzo szybko, jeśli wskaźnik myszy dotyka ważki. Sprawdzisz inny warunek, aby to naprawić.
</div>
<div>
![Scena przedstawiająca owada i ważkę.](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

Wybierz **ważkę** i znajdź skrypt, który zaczyna się od `po kliknięciu flagi`{:class="block3events"}.

Przeciągnij, `jeżeli`{:class="block3control"} do wnętrza bloku `zawsze`{:class="block3control"}, a bloki wewnątrz `zawsze`{:class="block3control"} przesuną się wewnątrz bloku, `jeżeli`{:class="block3control"}.

Sprawdź dokładnie, czy Twój kod wygląda tak:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if < > then
start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
end
```
--- /task ---

--- task ---

Następnie przeciągnij blok `nie`{:class="block3operators"} do `jeżeli`{:class="block3control"} i `dotyka (wskaźnik myszy)`{:class="block3sensing"} wewnątrz tego.

Sprawdź, czy Twój kod wygląda tak:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if <not <touching [mouse-pointer v] ?> > then
start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

Blok `nie`{:class="block3operators"} zmienia warunek w jego przeciwieństwo, tak jak w zdaniu.

--- /task ---

--- task ---

**Test:** Sprawdź, czy usterka została naprawiona i ważka porusza się tylko wtedy, gdy `nie`{:class="block3operators"} `dotyka (wskaźnik myszy)`{:class="block3sensing"}.

Innym warunkiem do wypróbowania jest:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

To sprawia, że ważka porusza się, gdy jest wystarczająco daleko od wskaźnika myszy.

**Wskazówka:** Możesz przeciągać bloki w dowolne miejsce w obszarze kodu i zostawiać je tam, próbując różnych rzeczy.

--- /task ---

--- save ---
