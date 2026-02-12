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

Drag an `if`{:class="block3control"} inside the `forever`{:class="block3control"} block. The blocks inside the `forever`{:class="block3control"} will move inside the `if`{:class="block3control"}.

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

Then drag a `not`{:class="block3operators"} block into the `if`{:class="block3control"} and a `touching (mouse-pointer)`{:class="block3sensing"} inside that.

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

--- /task ---

--- task ---

**Протестуй:** перевір, чи виправилась дивна поведінка бабки і чи вона рухається, лише якщо `не`{:class="block3operators"} `торкається (вказівника)`{:class="block3sensing"}.

--- /task ---

--- task ---

Try a different condition that makes the dragonfly move when it is far enough from the mouse-pointer:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

--- /task ---

--- save ---
