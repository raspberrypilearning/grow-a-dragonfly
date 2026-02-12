
--- question ---
---
legend: Питання 2 з 3
---

Твій код робить так, що бабка рухається тільки, якщо вона `не`{:class="block3operators"} `торкається`{:class="block3sensing"} вказівника миші.

Куди ти поставиш блок `відтворити звук`{:class="block3sound"}, щоб бабка відтворювала звук щоразу, як рухається?

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

Ні, з цим кодом блок `відтворити звук`{:class="block3sound"} знаходиться поза блоком `якщо`{:class="block3control"}, тому він запускатиметься щоразу, як починається цикл `завжди`{:class="block3control"}, навіть якщо бабка не рухається.

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

Так, правильно. Якщо розмістити блок `відтворити звук`{:class="block3sound"} всередині блоку `якщо`{:class="block3control"}, звук буде відтворюватися, коли бабка рухатиметься.

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

Ні, блок `відтворити звук`{:class="block3sound"} знаходиться поза блоком `якщо`{:class="block3control"}, тобто він запускатиметься щоразу, як починається цикл `завжди`{:class="block3control"}, навіть якщо бабка не рухається.

  --- /feedback ---

--- /choices ---

--- /question ---
