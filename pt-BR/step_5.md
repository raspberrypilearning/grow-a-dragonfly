## Movimento aprimorado

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
A libélula 'falha' e muda de direção muito rápido se o ponteiro do mouse estiver tocando a libélula. Você verificará outra condição para corrigir isso.
</div>
<div>
![O Stage mostrando um inseto e uma libélula.](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

Selecione o **Dragonfly** e encontre o script que começa com `quando o sinalizador clicou em`{:class="block3events"}.

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

**Teste:** Verifique se a falha foi corrigida, e o Dragonfly só se move quando `não`{:class="block3operators"} `touching (mouse-pointer)`{:class="block3sensing"}.

--- /task ---

--- task ---

Try a different condition that makes the dragonfly move when it is far enough from the mouse-pointer:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

--- /task ---

--- save ---
