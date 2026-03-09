## Pryfyn i'w fwyta

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Byddi di'n ychwanegu pryfyn i'r gwas-y-neidr gael ei fwyta. 
</div>
<div>
![Y Llwyfan gyda gwas y neidr a phryfyn.](images/fly-to-eat.png){:width="300px"}
</div>
</div>

Mae pry yn y corlun **Frog 2** y galli di ei ddefnyddio.

--- task ---

Ychwanega'r corlun **Frog 2** at dy brosiect. Ail-enwa'r corlun yn `Insect`:

![Y rhestr Corluniau gyda'r corlun Frog 2 wedi'i ychwanegu. Y briodwedd enw corlun yn dangos 'Insect'.](images/fly-sprite.png)


--- /task ---

Dim ond y pry sydd ei angen arnat ti, nid y broga.

--- task ---

Clicia'r tab **Gwisgoedd**. Clicia'r pry i'w ddewis a chlicio ar yr eicon **Copïo**.

![Y golygydd paent gyda rhan pry y wisg Frog 2-a wedi'i dewis a'r eicon Copïo wedi'i hamlygu.](images/copy-fly.png)

--- /task ---

--- task ---

Ychwanega wisg newydd i'r corlun drwy ddefnyddio'r opsiwn **Paentio**:

![Yr opsiwn paent wedi'i ddewis yn y ddewislen dewis gwisgoedd.](images/paint-sprite.png)

--- /task ---

--- task ---

Clicia ar yr eicon **Gludo** i ludo'r corlun i mewn i'r wisg newydd. Llusga'r pry i'r **canol** fel ei fod wedi'i alinio a'r groes.

Clicia ar yr eicon **Gludo** i ludo'r corlun i mewn i'r wisg newydd. Llusga'r pry i'r **canol** fel ei fod wedi'i alinio a'r groes.

![Y golygydd paent yn dangos gwisg Insect newydd wedi'i gludo gyda'r eicon Gludo wedi'i hamlygu. Y rhestr gwisgoedd yn dangos bod y gwisgoedd eraill wedi'u dileu.](images/fly-costume.png)

--- /task ---

--- task ---

Cynydda faint y pry fel ei fod yn haws ei weld a'i ddal:

![Y briodwedd Maint wedi'i gosod i 150.](images/fly-size.png)

--- /task ---

--- task ---

Clicia'r tab **Cod** ac ychwanegu sgript i wneud i'r corlun **Insect** fownsio o gwmpas:

![](images/fly-icon.png)

```blocks3
when flag clicked
forever
move [3] steps
if on edge, bounce
end
```

Mae'r bloc `os ar ymyl, bowndio`{:class="block3motion"} yn gwirio bloc i weld a yw'r corlun wedi cyrraedd ymyl y Llwyfan ac yn troi'r corlun i wynebu i gyfeiriad gwahanol os ydyw.

--- /task ---

Rwyt ti eisiau i'r corlun **Insect** `guddio`{:class="block3looks"} `os`{:class="block3control"} mae'n cael ei fwyta gan y corlun **Dragonfly**.

--- task ---

Ychwanega floc `os`{:class="block3control"} i sgript symud y corlun **Insect**:

```blocks3
when flag clicked
forever
move [3] steps
if on edge, bounce
+if < > then 
end
```
--- /task ---

Mae gan `os`{:class="block3control"} fewnbwn siâp hecsagon. Mae hyn yn golygu y galli di roi **amod** yma.

Pan fydd y bloc `os`{:class="block3control"} yn rhedeg, bydd Scratch yn gwirio'r amod. Os ydy'r cyflwr yn 'wir' `yna`{:class="block3control"} bydd y cod y tu mewn i'r bloc `os`{:class="block3control"} yn rhedeg.

Rwyt ti eisiau i'r pryfyn `guddio`{:class="block3looks"} `os`{:class="block3control"} mae'n `cyffwrdd`{:class="block3sensing"} y corlun **Dragonfly**.

--- task ---

Llusga `cyffwrdd [Dragonfly v]`{:class="block3sensing"} i mewn i'r bloc `os`{:class="block3control"}. Ychwanega floc `cuddio`{:class="block3looks"} y tu mewn i'r bloc `os`{:class="block3control"}.

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

**Profi:** Profa'r cod a rheola'r gwas-y-neidr i fwyta'r pry. Dylai'r pry ddiflannu.

--- /task ---

Fydd y gwas-y-neidr ddim yn tyfu'n fawr iawn os mai dim ond un pry mae'n gallu ei fwyta!

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

**Profi:** Profa fod dy was-y-neidr yn gallu bwyta llawer o bryfed bellach.

Make sure you have added the `show`{:class="block3looks"} block at the start.

--- /task ---

**Awgrym:** Galli di glicio ar y botwm **Aros** coch uwchben y Llwyfan os wyt ti am i'r gwas-y-neidr fod yn dawel wrth i ti ychwanegu mwy o god.

--- save ---
