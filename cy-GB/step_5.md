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

Llusga floc `os`{:class="block3control"} y tu mewn i'r bloc `am byth`{:class="block3control"} a bydd y blociau y tu mewn i'r bloc `am byth`{:class="block3control"} yn symud y tu mewn i'r bloc `os`{:class="block3control"}.

Gwiria yn ofalus fod dy god yn edrych fel hyn:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if < > then
start sound [Adenydd v]
point towards (mouse-pointer v)
move [5] steps
end
end
```
--- /task ---

--- task ---

Yna llusga floc `nid`{:class="block3operators"} i mewn i'r bloc `os`{:class="block3control"} a bloc `cyffwrdd (pwyntydd y llygoden)`{:class="block3sensing"} y tu mewn i hwnnw.

Gwna'n siŵr fod dy god yn edrych fel hyn:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if <not <touching [mouse-pointer v] ?> > then
start sound [Adenydd v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

Mae'r bloc `nid`{:class="block3operators"} yn troi amod i'r gwrthwyneb, yn union fel y byddai mewn brawddeg.

--- /task ---

--- task ---

**Profi:** Gwna'n siŵr fod y broblem wedi'i thrwsio, ac mai dim ond pan `nid`{:class="block3operators"} yn `cyffwrdd (pwyntydd y llygoden)`{:class="block3sensing"} y bydd y Gwas-y-neidr yn symud.

Amod gwahanol i roi cynnig arno yw:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

Mae hyn yn gwneud i'r gwas-y-neidr symud pan fydd yn ddigon pell o bwyntydd y llygoden.

**Awgrym:** Galli di lusgo blociau unrhyw le yn ardal y Cod a'u gadael yno wrth roi cynnig ar wahanol bethau.

--- /task ---

--- save ---
