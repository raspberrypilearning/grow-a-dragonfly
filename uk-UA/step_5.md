## Покращений рух

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Бабка «глючить» і дуже швидко змінює напрямок, якщо вказівник миші торкається бабки. Ти додаси ще одну умову, щоб це виправити.
</div>
<div>
![Сцена, що показує комаху й бабку.](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

Вибери спрайт **Dragonfly** і знайди скрипт, який починається блоком `коли прапорець натиснуто`{:class="block3events"}.

Перетягни блок `якщо`{:class="block3control"} всередину блока `завжди`{:class="block3control", і блоки всередині `завжди`{:class="block3control"} перейдуть усередину `якщо`{:class="block3control"}.

Твій код має виглядати так:

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

Потім перетягни блок `не`{:class="block3operators"} у блок `якщо`{:class="block3control"}, а всередину `не`{:class="block3operators"} перемісти блок `торкається (вказівник)`{:class="block3sensing"}.

Твій код має виглядати так:

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

Блок `не`{:class="block3operators"} перетворює умову на зворотну, як і у реченні.

--- /task ---

--- task ---

**Протестуй:** перевір, чи виправилась дивна поведінка бабки і чи вона рухається, лише якщо `не`{:class="block3operators"} `торкається (вказівника)`{:class="block3sensing"}.

Ти також можеш спробувати таку умову:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

Вона змушує бабку рухатися, коли вона знаходиться на достатній відстані від вказівника миші.

**Порада:** ти можеш перетягувати блоки в будь-яке місце в області коду й залишати їх там, поки пробуєш різні варіанти.

--- /task ---

--- save ---
