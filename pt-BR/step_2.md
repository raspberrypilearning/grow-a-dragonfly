## Preparando o cenário

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Você vai definir a cena. Escolha sua imagem de fundo e adicione uma libélula que segue o ponteiro do mouse ao redor do cenario.
</div>
<div>
![Libélula em fundo desértico](images/set-the-scene.png){:width="300px"}
</div>
</div>

--- task ---

Abra o [projeto inicial Cresça uma libélula](https://scratch.mit.edu/projects/535695413/editor){:target="_ blank"}. Scratch will open a blank project in a new browser tab.

--- /task ---

--- task ---

Click **Choose a Backdrop** and add a backdrop of your choice. Usamos o cenário **Jurassic**.

![Ícone de Backdrop na interface do aplicativo Scratch](images/choose-backdrop-icon.png)

![O Palco mostrando o cenário jurassic.](images/Jurassic-backdrop.png)

--- /task ---

--- task ---

Clique em **Escolha um Sprite** e procure por `dragonfly`, então adicione o sprite **Dragonfly**.

![Ícone Sprite na interface do app Scratch](images/choose-sprite-icon.png)

![A caixa de pesquisa com 'libélula' digitada e o sprite da libélula na galeria.](images/dragonfly-search.png)

--- /task ---

--- task ---

Adicione um script para fazer o sprite **Dragonfly** seguir o ponteiro do mouse (ou seu dedo):

![Ícone do sprite Dragonfly na interface do app Scratch](images/dragonfly-icon.png)

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

**Teste:** Clique na bandeira verde e faça o sprite **Dragonfly** se mover pelo cenario. A libélula está se movendo como você esperava?

--- /task ---

O traje Dragonfly não está voltado para a direita, então a cabeça do sprite **Dragonfly** não está apontando para o ponteiro do mouse.

--- task ---

Clique na aba **Costumes** e use a ferramenta **Select** (seta) para selecionar a fantasia.

Use a ferramenta **Rotate** na parte inferior do traje selecionado para virar o traje **Dragonfly** para a direita.

![Uma imagem animada mostrando como girar a fantasia de libélula arrastando as setas de rotação para que a libélula fique voltada para a direita.](images/rotated-costume.gif)

--- /task ---

--- task ---

**Teste:** Clique na bandeira verde e veja como a libélula se move agora.

--- /task ---

As asas da libélula fazem um som esvoaçante enquanto vibram. Você pode editar um som no Scratch para criar seu próprio som.

--- task ---

Adicione o som **Crank** ao sprite **Dragonfly**.

[[[generic-scratch3-sound-from-library]]]

![](images/crank-sound-editor.png)

--- /task ---

--- task ---

**Test:** Click the **Play** button so you can hear the sound.

--- /task ---

O som **Crank** é muito longo e muito lento para asas de libélula.

--- task ---

Selecione o final do som usando o cursor ou o dedo.

Clique em **Copy to New** para criar um novo som apenas com a parte selecionada:

![O final do som de crank selecionado em azul com o ícone 'Copiar para novo' realçado.](images/crank-copy-end.png)

--- /task ---

--- task ---

Renomeie seu novo som de **Crank2** para `Wings`. ![A propriedade renomear sons.](images/crank-wings-sound.png)

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
