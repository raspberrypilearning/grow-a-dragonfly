## Gosod yr olygfa

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Byddi di'n gosod y cyd-destun. Dewisa dy gefnlen ac ychwanegu gwas-y-neidr sy'n dilyn pwyntydd y llygoden o amgylch y Llwyfan.
</div>
<div>
![](images/set-the-scene.png){:width="300px"}
</div>
</div>

--- task ---

Agora'r prosiect cychwynnol [Tyfu gwas-y-neidr](https://scratch.mit.edu/projects/535695413/editor){:target="_blank"}. Scratch will open a blank project in a new browser tab.

--- /task ---

--- task ---

Click **Choose a Backdrop** and add a backdrop of your choice. Rydyn ni wedi defnyddio'r gefnlen **Jurassic**.

![Backdrop icon on the Scratch app interface](images/choose-backdrop-icon.png)

![Y Llwyfan yn dangos y gefnlen Jurassic.](images/Jurassic-backdrop.png)

--- /task ---

--- task ---

Clicia **Dewiswch Gorlun** a chwilia am `dragonfly`, wedyn ychwanegu'r corlun **Dragonfly**.

![Sprite icon on the Scratch app interface](images/choose-sprite-icon.png)

![Y blwch chwilio gyda 'dragonfly' wedi'i deipio i mewn a'r corlun Dragonfly yn yr oriel.](images/dragonfly-search.png)

--- /task ---

--- task ---

Ychwanega sgript i wneud i'r corlun **Dragonfly** ddilyn pwyntydd y llygoden (neu dy fys):

![Dragonfly sprite icon on the Scratch app interface](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] % // to start small
forever
point towards (mouse-pointer v)
move [5] steps
end
```
--- /task ---

--- task ---

**Profi:** Clicia'r faner werdd a gwnud i'r corlun **Dragonfly** symud o amgylch y Llwyfan. Ydy'r gwas-y-neidr yn symud fel y byddet ti'n ei ddisgwyl?

--- /task ---

Dydy'r wisg Dragonfly ddim yn wynebu i'r dde, felly dydy pen y corlun **Dragonfly** ddim yn pwyntio at bwyntydd y llygoden.

--- task ---

Cliciwch ar y tab **Gwisgoedd** a defnyddia'r offeryn **Dewis** (saeth) i ddewis y wisg.

Defnyddia'r offeryn **Cylchdroi** ar waelod y wisg a ddewiswyd i droi'r wisg **Dragonfly** i wynebu'r dde.

![Delwedd animeiddiedig yn dangos sut i gylchdroi'r wisg dragonfly drwy lusgo'r saethau cylchdroi fel bod y gwas y neidr yn wynebu i'r dde.](images/rotated-costume.gif)

--- /task ---

--- task ---

**Profi:** Clicia'r faner werdd ac edrycha sut mae'r gwas-y-neidr yn symud nawr.

--- /task ---

Mae adenydd gwas-y-neidr yn gwneud sŵn siffrwd wrth iddynt ddirgrynu. Galli di olygu sain yn Scratch i greu dy sain dy hun.

--- task ---

Ychwanega'r sain **Crank** at y corlun **Dragonfly**.

[[[generic-scratch3-sound-from-library]]]

![](images/crank-sound-editor.png)

--- /task ---

--- task ---

Clicia'r botwm **Chwarae** er mwyn i ti allu clywed y sain.

--- /task ---

Mae'r sain **Crank** yn rhy hir ac yn rhy araf ar gyfer adenydd gwas-y-neidr.

--- task ---

Dewisa ddiwedd y sain gan ddefnyddio'ch cyrchwr neu dy fys.

Clicia **Copïo i'r Newydd** i greu sain newydd gyda'r rhan a ddewiswyd yn unig:

![Diwedd y sain crank wedi'i ddewis mewn glas gyda'r eicon 'Copïo i'r Newydd' wedi'i hamlygu.](images/crank-copy-end.png)

--- /task ---

--- task ---

Newidia enw dy sain newydd o **Crank2** i `Adenydd`. ![Y briodwedd rename sound.](images/crank-wings-sound.png)

--- /task ---

--- task ---

**Test:** Play the new sound. Click the **Faster** button a few times until you like the result:

![A faster sound wave with the 'Faster' icon highlighted.](images/wings-faster.png)

--- /task ---

--- task ---

If you like, you can select the very end of the **Wings** sound, and then click **Delete** to remove it:

![The end of the sound wave selected with the 'Delete' tool highlighted.](images/wings-shorter.png)

--- /task ---

--- task ---

Now add a block to play the **Wings** sound when the dragonfly moves:

![Dragonfly sprite icon](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
```
--- /task ---

--- task ---

**Test:** Try out your dragonfly movement and sound effect.

--- /task ---

--- save ---
