## Symud yn well

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Bydd y gwas-y-neidr yn 'nogio' ac yn newid ei gyfeiriad yn gyflym iawn os ydy pwyntydd y llygoden yn cyffwrdd â'r gwas-y-neidr. Byddi di'n gwirio amod arall i ddatrys hyn.
</div>
<div>
![Y Llwyfan yn dangos pryfyn a gwas-y-neidr.](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

Dewisa'r **Gwas-y-neidr** a chwilia am y sgript sy'n dechrau gyda `pan fydd y faner wedi'i chlicio`{:class="block3events"}.

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

**Profi:** Gwna'n siŵr fod y broblem wedi'i thrwsio, ac mai dim ond pan `nid`{:class="block3operators"} yn `cyffwrdd (pwyntydd y llygoden)`{:class="block3sensing"} y bydd y Gwas-y-neidr yn symud.

--- /task ---

--- task ---

Try a different condition that makes the dragonfly move when it is far enough from the mouse-pointer:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

--- /task ---

--- save ---
