## Повний розмір

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Ти зробиш так, щоб бабка росла, коли зʼїдає муху, і переставала рости, коли досягне повного розміру.
</div>
<div>
![Повнорозмірна бабка на Сцені каже: «Я досягла повного розміру!».](images/grow-to-fullsize.png){:width="300px"}
</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
Найбільші бабки у природі живуть у Центральній Америці. Розмах їхніх крилець становить 19 см (трохи більше за твою долоню). Найбільшою комахою, що колись існувала, була <span style="color: #0faeb0">**Meganeuropsis permiana**</span> (меганевро́псис перміáна), бабка з розмахом крилець у 75 см (як довжина великого кроку).</p>

Муха знає, що її з'їли, а тепер бабці потрібно знати, щоб вона виросла.

Коли ти хочеш повідомити іншому спрайту, що щось сталося, ти можеш використати блок `оповістити`{:class="block3events"}, як у проєкті [Чарівні оповіщення](https://projects.raspberrypi.org/uk-UA/projects/broadcasting-spells){:target="_blank"}.

--- task ---

Додай блок `оповістити`{:class="block3events"} до спрайта **Комаха** з новим повідомленням `їжа`{:class="block3events"}:

![](images/fly-icon.png)

```blocks3
when flag clicked
show // показувати на початку
forever
move [3] steps
if on edge, bounce
if <touching [Dragonfly v] ?> then
+broadcast [їжа v]
hide
go to (випадкова позиція v)
wait [1] seconds
show
end
end
```
--- /task ---

Спрайт **Dragonfly** має вирости, коли отримає повідомлення `їжа`{:class="block3events"}.

--- task ---

Вибери спрайт **Dragonfly** і додай такий скрипт:

![](images/dragonfly-icon.png)

```blocks3 
when I receive [їжа v]
change size by [5]
```

--- /task ---

--- task ---

Додай звук **Chomp** до бабки і `відтвори`{:class="block3sound"} його, коли бабка зʼїдає комаху:

![](images/dragonfly-icon.png)

```blocks3 
when I receive [їжа v]
+start sound [Chomp v]
change size by [5]
```
--- /task ---

--- task ---

**Протестуй:** запусти свій проєкт, щоб перевірити, як бабка виростає і відтворює звук поглинання їжі, коли зʼїдає муху.

--- /task ---

Коли бабка досягне повного розміру, гра привітає тебе і зупиниться.

--- task ---

Додай блок `якщо`{:class="block3control"}.

Бабка досягне повного розміру, коли `розмір`{:class="block3looks"} `=`{:class="block3operators"} `100%`. Насамперед додай оператор `=`{:class="block3operators"} у шестикутне поле введення:

![](images/dragonfly-icon.png)

```blocks3
when I receive [їжа v]
start sound [Chomp v]
change size by [5]
+if <[ ] = [ ]> then
end
```
--- /task ---

--- task ---

Заверши побудову умови за допомогою вбудованої змінної `розмір`{:class="block3looks"}, ввівши значення `100`:

![](images/dragonfly-icon.png)

```blocks3
when I receive [їжа v]
start sound [Chomp v]
change size by [5]
+if <(size) = [100]> then
end
```
--- /task ---

--- task ---

Додай блоки, щоб відбувалося наступне: `якщо`{:class="block3control"} умова справджується, `то`{:class="block3control"} бабка `оповістить`{:class="block3events"} за допомогою повідомлення «кінець» і `скаже`{:class="block3looks"} `Я досягла повного розміру!`

Наприкінці додай блок `зупинити все`{:class="block3control"}, щоб зупинити решту скриптів бабки:

![](images/dragonfly-icon.png)

```blocks3
when I receive [їжа v]
start sound [Chomp v]
change size by [5]
if <(size) = [100]> then
+broadcast [кінець v]
+say [Я досягла повного розміру!]
+stop [інші скрипти цього спрайту v] // зміни зі «все»
end
```
--- /task ---

--- task ---

Зараз муха продовжує рухатися після закінчення проєкту. Додай цей скрипт до спрайта **Комаха**.

![](images/fly-icon.png)

```blocks3
when I receive [кінець v]
stop [інші скрипти цього спрайту v]
```

--- /task ---

--- task ---

**Протестуй:** клікни на зелений прапорець і продовжуй їсти мух, доки твоя бабка не досягне повного розміру.

--- /task ---

--- save ---
