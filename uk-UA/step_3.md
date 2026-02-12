## Смачна муха

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Ти додаси комаху, яку бабка зможе зʼїсти. 
</div>
<div>
![Сцена з бабкою і комахою.](images/fly-to-eat.png){:width="300px"}
</div>
</div>

У спрайті **Frog 2** є муха, яку ти можеш використати.

--- task ---

Додай спрайт **Frog 2** («жаба 2») до свого проєкту. Зміни назву спрайта на `Комаха`:

![Список спрайтів із доданим спрайтом Frog 2 («Жаба 2»). У полі з назвою спрайта вказано «Комаха».](images/fly-sprite.png)


--- /task ---

Тобі потрібна тільки комаха без жаби.

--- task ---

Перейди до вкладки **Образи**. Натисни на муху, щоб вибрати її, та клікни по іконці **Копія**.

![Редактор Малювання з мухою — частиною образу Frog 2-a — та підсвіченою іконкою «Копія».](images/copy-fly.png)

--- /task ---

--- task ---

Додай новий образ до спрайта, використовуючи функцію **Малювати**:

![Виділена функція малювання у меню вибору образу.](images/paint-sprite.png)

--- /task ---

--- task ---

Натисни на іконку **Вставити**, щоб вставити спрайт у новий образ. Перетягни муху до **центру**, щоб вона зрівнялася з прицілом.

Rename your costume `Insect` and delete the other costumes, as you won't need those:

![Редактор Малювання зі вставленим новим образом комахи та підсвіченою іконкою «Вставити». Список образів показує, що решту образів було видалено.](images/fly-costume.png)

--- /task ---

--- task ---

Збільш розмір мухи, щоб її було легше побачити і зловити:

![Розмір встановлено на 150.](images/fly-size.png)

--- /task ---

--- task ---

Перейди до вкладки **Код** і додай скрипт, за допомогою якого спрайт **Комаха** стрибатиме Сценою:

![](images/fly-icon.png)

```blocks3
when flag clicked
forever
move [3] steps
if on edge, bounce
end
```

Блок `якщо на межі, відбити`{:class="block3motion"} перевіряє, чи спрайт дійшов до межі Сцени, і, якщо так, розвертає спрайт в інший напрямок.

--- /task ---

Тобі потрібно, щоб спрайт **Комаха** `сховався`{:class="block3looks"}, `якщо`{:class="block3control"} його зʼїдає спрайт **Dragonfly** («бабка»).

--- task ---

Додай блок `якщо`{:class="block3control"} до скрипту руху спрайта **Комаха**:

```blocks3
when flag clicked
forever
move [3] steps
if on edge, bounce
+if < > then 
end
```
--- /task ---

Блок `якщо`{:class="block3control"} має шестикутне поле вводу. Це означає, що ти можеш вставити туди **умову**.

Коли запускатиметься блок `якщо`{:class="block3control"}, Скретч перевірятиме цю умову. Якщо умова справджується, `то`{:class="block3control"} запуститься код всередині блока `якщо`{:class="block3control"}.

Тобі потрібно, щоб комаха `сховалась`{:class="block3looks"}, `якщо`{:class="block3control"} вона `торкається`{:class="block3sensing"} спрайта **Dragonfly**.

--- task ---

Перетягни блок `торкається [Dragonfly v]`{:class="block3sensing"} всередину блока `якщо`{:class="block3control"}. Додай блок `сховати`{:class="block3looks"} всередину блока `якщо`{:class="block3control"}.

```blocks3
when flag clicked
forever
move [3] steps
if on edge, bounce
+if <touching [Dragonfly v] ?> then // change from 'mouse-pointer'
+hide // eaten
end
```

--- /task ---

--- task ---

**Протестуй:** перевір свій код і спрямуй бабку так, щоб вона зʼїла муху. Муха має зникнути.

--- /task ---

Бабка не виросте дуже великою, якщо зʼїсть лише одну муху!

--- task ---

Add blocks to make the hidden insect sprite `go to a random position`{:class="block3motion"} on the Stage, `wait`{:class="block3control"} for one second then `show`{:class="block3looks"}:

```blocks3
when flag clicked
+show // show at the start
forever
move [3] steps
if on edge, bounce
if <touching [Dragonfly v] ?> then
hide
+go to (random position v)
+wait [1] seconds
+show // to look like a new fly
end
end
```

--- /task ---

--- task ---

**Протестуй:** переконайся, що тепер твоя бабка може зʼїсти багато мух.

Make sure you have added the `show`{:class="block3looks"} block at the start.

--- /task ---

**Порада:** ти можеш натиснути на червону кнопку **Зупинити** над Сценою, якщо ти хочеш, щоб бабка не стрекотала, поки ти додаєш код.

--- save ---
