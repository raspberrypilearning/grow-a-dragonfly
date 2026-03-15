## Crescer ao máximo

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Você fará a libélula crescer quando comer uma mosca e parar ao atingir o tamanho maximo.
</div>
<div>
![A libélula em tamanho maximo no Stage dizendo 'Cheguei ao tamanho maximo!'.](images/grow-to-fullsize.png){:width="300px"}
</div>
</div>

The Dragonfly needs to grow when it eats a fly.

Quando você precisar avisar outro sprite que algo aconteceu, você pode usar um bloco `broadcast`{:class="block3events"} como você fez em [Broadcasting spells](https://projects.raspberrypi.org/en/projects/broadcasting-spells){:target="_blank"}.

--- task ---

Adicione um bloco `broadcast`{:class="block3events"} ao sprite **Insect** com a nova mensagem `food`{:class="block3events"}:

![](images/fly-icon.png)

```blocks3
when flag clicked
show // show at the start
forever
move [3] steps
if on edge, bounce
if <touching [Dragonfly v] ?> then
+broadcast [food v]
hide
go to (random position v)
wait [1] seconds
show
end
end
```
--- /task ---

O sprite **Dragonfly** precisa crescer quando receber a mensagem `food`{:class="block3events"}.

--- task ---

Selecione o sprite **Dragonfly** e adicione este script:

![](images/dragonfly-icon.png)

```blocks3 
when I receive [food v]
change size by [5]
```

--- /task ---

--- task ---

Adicione o som **Chomp** à libélula e `inicie`{:class="block3sound"} quando um inseto for comido:

```blocks3 
when I receive [food v]
+start sound [Chomp v]
change size by [5]
```
--- /task ---

--- task ---

**Teste:** Execute seu projeto para testar se a libélula cresce e faz um som de mastigação quando come uma mosca.

--- /task ---

Quando a libélula atingir seu tamanho máximo, o jogo irá parabenizá-lo e parar.

--- task ---

Adicione um bloco `if`{:class="block3control"}.

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
+if < > then
end
```

--- /task ---

A libélula fica no tamanho maximo quando `tamanho`{:class="block3looks"} `=`{:class="block3operators"} `100%`.

--- task ---

First, add an `=`{:class="block3operators"} operator into the hexagon-shaped input:

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
+if <[ ] = [ ]> then
end
```
--- /task ---

--- task ---

Conclua a construção da condição adicionando uma variável `size`{:class="block3looks"} integrada e digite o valor `100`:

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
+if <(size) = [100]> then
end
```
--- /task ---

--- task ---

Adicione blocos para que `if`{:class="block3control"} a condição for verdadeira `then`{:class="block3control"} a libélula `transmitirá`{:class="block3events"} uma mensagem 'end' e `diga`{:class="block3looks"} `Cheguei ao tamanho maximo!`

Por fim, adicione um bloco `stop all`{:class="block3control"} para parar os outros scripts de libélula:

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
if <(size) = [100]> then
+broadcast [end v]
+say [I got to full size!]
+stop [other scripts in sprite v] // change from 'all'
end
```
--- /task ---

--- task ---

No momento, a mosca ainda se move após o término do projeto. Adicione este script ao sprite **Insect**.

![](images/fly-icon.png)

```blocks3
when I receive [end v]
stop [other scripts in sprite v]
```

--- /task ---

--- task ---

**Teste:** Clique na bandeira verde e continue comendo moscas até que sua libélula atinja o tamanho máximo.

--- /task ---

--- save ---
