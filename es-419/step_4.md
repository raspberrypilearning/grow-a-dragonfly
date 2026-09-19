## Que crezca a tamaño completo

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Harás que la libélula crezca cuando se coma una mosca, y se detendrá si alcanza su tamaño completo.
</div>
<div>
![La libélula de tamaño completo en el Escenario diciendo '¡He conseguido mi tamaño completo!'.](images/grow-to-fullsize.png){:width="300px"}
</div>
</div>

The Dragonfly needs to grow when it eats a fly.

Cuando necesites que otro objeto sepa que algo sucedió, puedes usar un bloque `enviar`{:class="block3events"} como lo hiciste en [Enviando hechizos](https://projects.raspberrypi.org/en/projects/broadcasting-spells){:target="_blank"}.

--- task ---

Agrega un bloque `enviar`{:class="block3events"} al objeto **Insecto** con el nuevo mensaje `comida`{:class="block3events"}:

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

El objeto **Dragonfly** necesita crecer cuando recibe el mensaje `comida`{:class="block3events"}.

--- task ---

Selecciona el objeto **Libélula** y agrega este script:

![](images/dragonfly-icon.png)

```blocks3 
when I receive [food v]
change size by [5]
```

--- /task ---

--- task ---

Agrega el sonido **Chomp** a la libélula e `iniciálo`{:class="block3sound"} cuando un insecto sea comido:

```blocks3 
when I receive [food v]
+start sound [Chomp v]
change size by [5]
```
--- /task ---

--- task ---

**Prueba:** Ejecuta tu proyecto para probar que la libélula crece y hace un sonido de mordisco cuando come una mosca.

--- /task ---

Cuando esta alcance su tamaño completo, el juego te felicitará y se detendrá.

--- task ---

Agrega un bloque `si`{:class="block3control"}.

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
+if < > then
end
```

--- /task ---

La libélula es de tamaño completo cuando el `tamaño`{:class="block3looks"} `=`{:class="block3operators"} `100%`.

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

Termina de crear la condición agregando una variable personalizada para el `tamaño`{:class="block3looks"} y escribe el valor `100`:

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
+if <(size) = [100]> then
end
```
--- /task ---

--- task ---

Agregue bloques de modo que `si`{:class="block3control"} la condición es cierta `entonces`{:class="block3control"} la libélula va a `enviar`{:class="block3events"} un mensaje de 'fin' y va a `decir`{:class="block3looks"} `¡He conseguido mi tamaño completo!`

Finalmente, agrega un bloque `detener todos`{:class="block3control"} para detener los otros scripts de la libélula:

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

En este momento, la mosca sigue moviéndose una vez finalizado el proyecto. Agrega este script al objeto **Insecto**.

![](images/fly-icon.png)

```blocks3
when I receive [end v]
stop [other scripts in sprite v]
```

--- /task ---

--- task ---

**Prueba:** Pulsa en la bandera verde y sigue comiendo moscas hasta que tu libélula alcance su tamaño completo.

--- /task ---

--- save ---
