
--- question ---
---
legend: Question 2 of 3
---

Você escreveu o código para fazer a libélula se mover apenas se for `not/0>{:class="block3operators"} <code>tocando`{:class="block3sensing"} o ponteiro do mouse.

Onde você colocaria um bloco `start sound`{:class="block3sound"} para fazer a libélula iniciar um som cada vez que se move?

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

Não, com este código o bloco `start sound`{:class="block3sound"} está fora do bloco `if`{:class="block3control"}, então ele será executado toda vez que o bloco `forever`{:class=" block3control"} é executado, mesmo que a libélula não se mova.

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

Sim esta correto. Colocar o bloco `start sound`{:class="block3sound"} dentro do bloco `if`{:class="block3control"} significa que ele tocará quando a libélula se mover.

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

Não, o bloco `start sound`{:class="block3sound"} está fora do bloco `if`{:class="block3control"}, então ele será executado toda vez que o bloco `forever`{:class="block3control"} loop é executado, mesmo que a libélula não se mova.

  --- /feedback ---

--- /choices ---

--- /question ---
