## Tyfu i llawn faint

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Byddi di'n gwneud i'r gwas-y-neidr dyfu pan fydd yn bwyta pry, a stopio os bydd yn cyrraedd maint llawn.
</div>
<div>
![Gwas-y-neidr llawn ei faint ar y Llwyfan yn dweud 'Dw i 'di cyrraedd fy maint llawn!'.](delweddau/grow-to-fulsize.png){:width="300px"}
</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
Mae'r gweision y neidr byw mwyaf i'w cael yng Nghanolbarth America ac mae ganddyn nhw led adenydd o 19cm (ychydig yn fwy na dy law di). Y pryfyn mwyaf y gwyddom amdano erioed oedd <span style="color: #0faeb0">**Meganeuropsis permiana**</span>, gwas-y-neidr gyda lled adenydd tua 75cm (maint cam mawr).</p>

Mae'r pry yn gwybod ei fod wedi'i fwyta, a nawr mae angen i'r Gwas-y-neidr wybod er mwyn iddo dyfu.

Pan fyddi di angen rhoi gwybod i gorlun arall bod rhywbeth wedi digwydd, galli di ddefnyddio bloc `darlledu`{:class="block3events"} fel wnes di yn [Darlledu swynion](https://projects.raspberrypi.org/cy-GB/projects/broadcasting-spells){:target="_blank"}.

--- task ---

Ychwanega floc `darlledu`{:class="block3events"} i'r corlun **Insect** gyda neges newydd `bwyd`{:class="block3events"}:

![](images/fly-icon.png)

```blocks3
when flag clicked
show // dangos ar y dechrau
forever
move [3] steps
if on edge, bounce
if <touching [Dragonfly v] ?> then
+broadcast [bwyd v]
hide
go to (random position v)
wait [1] seconds
show
end
end
```
--- /task ---

Mae angen i'r corlun **Dragonfly** dyfu pan fydd yn derbyn y neges `bwyd`{:class="block3events"}.

--- task ---

Dewisa'r corlun **Dragonfly** ac ychwanegu'r sgript yma:

![](images/dragonfly-icon.png)

```blocks3 
when I receive [bwyd v]
change size by [5]
```

--- /task ---

--- task ---

Ychwanega'r sain **Chomp** at y gwas-y-neidr a `dechrau`{:class="block3sound"} pan fydd pryfyn yn cael ei fwyta:

![](images/dragonfly-icon.png)

```blocks3 
when I receive [bwyd v]
+start sound [Chomp v]
change size by [5]
```
--- /task ---

--- task ---

**Profi:** Rheda dy brosiect i brofi bod y gwas-y-neidr yn tyfu ac yn gwneud sain chomp wrth fwyta pryfyn.

--- /task ---

Pan fydd y gwas-y-neidr yn cyrraedd ei faint llawn, bydd y gêm yn dy longyfarch ac yn stopio.

--- task ---

Ychwanega floc `os`{:class="block3control"}.

Bydd y gwas-y-neidr yn cyrraedd ei faint llawn pan fydd y `maint`{:class="block3looks"} `=`{:class="block3operators"} `100%`. Yn gyntaf, ychwanega weithredwr `=`{:class="block3operators"} i'r mewnbwn siâp hecsagon:

![](images/dragonfly-icon.png)

```blocks3
when I receive [bwyd v]
start sound [Chomp v]
change size by [5]
+if <[ ] = [ ]> then
end
```
--- /task ---

--- task ---

Galli di orffen llunio'r amod drwy ychwanegu newidyn `maint`{:class="block3looks"} parod a theipio'r gwerth `100`:

![](images/dragonfly-icon.png)

```blocks3
when I receive [bwyd v]
start sound [Chomp v]
change size by [5]
+if <(size) = [100]> then
end
```
--- /task ---

--- task ---

Ychwanega flociau sy'n pennu `os`{:class="block3control"} yw'r cyflwr yn wir `yna`{:class="block3control"} bydd y gwas-y-neidr yn `darlledu`{:class="block3events"} neges 'diwedd' ac yn `dweud`{:class="block3looks"} `Dw i 'di cyrraedd fy maint llawn!`

Yn olaf, ychwanega floc `aros y cyfan`{:class="block3control"} i stopio'r sgriptiau gwas-y-neidr eraill:

![](images/dragonfly-icon.png)

```blocks3
when I receive [bwyd v]
start sound [Chomp v]
change size by [5]
if <(size) = [100]> then
+broadcast [diwedd v]
+say [Dw i 'di tyfu'n llawn!]
+stop [other scripts in sprite v] // newid o 'y cyfan'
end
```
--- /task ---

--- task ---

Ar hyn o bryd, mae'r pry yn dal i symud ar ôl i'r prosiect ddod i ben. Ychwanega'r sgript yma at y corlun **Insect**.

![](images/fly-icon.png)

```blocks3
when I receive [diwedd v]
stop [other scripts in sprite v]
```

--- /task ---

--- task ---

**Profi:** Clicia'r faner werdd a dalia ati i fwyta pryfed nes bod dy was-y-neidr yn cyrraedd ei faint llawn.

--- /task ---

--- save ---
