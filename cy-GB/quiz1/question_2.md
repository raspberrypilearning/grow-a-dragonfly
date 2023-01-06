
--- question ---
---
legend: Cwestiwn 2 o 3
---

Fe wnes ti ysgrifennu cod i wneud i'r gwas-y-neidr symud dim ond pan `na fydd`{:class="block3operators"} pwyntydd y llygoden yn `cyffwrdd`{:class="block3sensing"} ag ef.

Ble fydde ti'n rhoi bloc `cychwyn sain`{:class="block3sound"} i wneud i'r gwas-y-neidr wneud sŵn bob tro cyn iddo ddechrau symud?

--- choices ---

- ( )

```blocks3
when flag clicked
forever
+start sound [Adenydd v]
if <not <touching [mouse-pointer v] ?> > then
point towards (mouse-pointer v)
move [5] steps
end
end
```

--- feedback ---

Na, gyda'r cod hwn bydd y bloc `cychwyn sain`{:class="block3sound"} y tu allan i'r bloc `os`{:class="block3control"}, felly bydd yn rhedeg bob tro bydd y ddolen `am byth`{:class="block3control"} yn rhedeg, hyd yn oed os na fydd y gwas-y-neidr yn symud.

--- /feedback ---

- (x)

```blocks3
when flag clicked
forever
if <not <touching [mouse-pointer v] ?> > then
+start sound [Adenydd v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

  --- feedback ---

Cywir! Bydd gosod y bloc `cychwyn sain`{:class="block3sound"} y tu mewn i'r bloc `os`{:class="block3control"} yn golygu y bydd yn chwarae pan fydd y gwas-y-neidr yn symud.

  --- /feedback ---

- ( )


```blocks3
when flag clicked
forever
if <not <touching [mouse-pointer v] ?> > then
point towards (mouse-pointer v)
move [5] steps
end
+start sound [Adenydd v]
end
```

  --- feedback ---

Na. Mae'r bloc sain `cychwyn sain`{:class="block3sound"} y tu allan i'r bloc `os`{:class="block3control"}, felly bydd yn rhedeg bob tro y bydd y ddolen `am byth`{:class="block3control"} yn rhedeg, hyd yn oed os nad yw'r gwas-y-neidr yn symud.

  --- /feedback ---

--- /choices ---

--- /question ---
