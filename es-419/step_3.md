## Una mosca para comer

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Agregarás un insecto para que la libélula lo coma. 
</div>
<div>
![El escenario con una libélula y un insecto.](images/fly-to-eat.png){:width="300px"}
</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
Los personajes que se mueven solos en los juegos a veces se denominan <span style="color: #0faeb0">**mobs**</span>, abreviatura de móviles. ¿Puedes pensar en un juego que tenga mobs?</p>

Hay una mosca en el objeto **Frog 2** que puedes usar.

--- task ---

Agrega el objeto **Frog 2** a tu proyecto. Cambia el nombre del objeto a `Insecto`:

![La Lista de objetos con el objeto Frog 2 añadido. La propiedad nombre del Objeto muestra 'Insecto'.](images/fly-sprite.png)


--- /task ---

Solo necesitas la mosca, no la rana.

--- task ---

Pulsa en la pestaña **Disfraces**. Pulsa sobre la mosca para seleccionarla y pulsa en el icono **Copiar**.

![El editor de pintura con la parte de la mosca de Frog 2- un disfraz seleccionado y el ícono Copiar resaltado.](images/copy-fly.png)

--- /task ---

--- task ---

Agrega un nuevo disfraz al objeto usando la opción **Pintar**:

![La opción pintar seleccionada en el menú elegir un disfraz.](images/paint-sprite.png)

--- /task ---

--- task ---

Pulsa en el icono **Pegar** para pegar el objeto en el nuevo disfraz. Arrastra la mosca al **centro** para que se alinee con la cruz.

Puedes cambiar el nombre de tu disfraz `Insecto` y eliminar los otros disfraces, ya que no los necesitarás:

![El editor de pintura que muestra un nuevo disfraz de Insecto pegado con el ícono Pegar resaltado. La lista de disfraces muestra que se han eliminado los otros disfraces.](images/fly-costume.png)

--- /task ---

--- task ---

Aumenta el tamaño de la mosca para que sea más fácil de ver y atrapar:

![Propiedad de tamaño establecida en 150.](images/fly-size.png)

--- /task ---

--- task ---

Pulsa en la pestaña **Código** y agrega un script para hacer que el objeto **Insecto** rebote alrededor:

![](images/fly-icon.png)

```blocks3
when flag clicked
forever
move [3] steps
if on edge, bounce
end
```

El bloque `si toca un borde, rebotar`{:class="block3motion"} comprueba si el objeto ha llegado al borde del Escenario y apunta el objeto hacia una dirección diferente si la tiene.

--- /task ---

Quieres que el objeto **Insecto** se `esconda`{:class="block3looks"} `si`{:class="block3control"} es comido por el objeto **Dragonfly**.

--- task ---

Agrega un bloque `si`{:class="block3control"} al script de movimiento del objeto **Insecto**:

![](images/fly-icon.png)

```blocks3
when flag clicked
forever
move [3] steps
if on edge, bounce
+if < > then 
end
```
--- /task ---

El `si`{:class="block3control"} tiene una entrada en forma de hexágono. Esto significa que puedes poner una **condición** aquí.

Cuando se ejecuta el bloque `si`{:class="block3control"}, Scratch verificará la condición. Si la condición es 'verdadera' `entonces`{:class="block3control"} se ejecutará el código dentro del bloque `if`{:class="block3control"}.

Quieres que el insecto se `esconda`{:class="block3looks"} `si`{:class="block3control"} está `tocando`{:class="block3sensing"} el objeto **Dragonfly**.

--- task ---

Arrastra un `tocando [Dragonfly v]`{:class="block3sensing"} al bloque `si`{:class="block3control"}. Agrega un bloque `esconder`{:class="block3looks"} dentro del bloque `if`{:class="block3control"}.

![](images/fly-icon.png)

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

**Prueba:** Ensaya tu código y controla la libélula para que se coma la mosca. La mosca debería desaparecer.

--- /task ---

¡La libélula no crecerá mucho si solo puede comer una mosca!

--- task ---

Agrega los bloques `ir a posición aleatoria`{:class="block3motion"} en el Escenario, y haz que tu objeto `espere`{:class="block3control"} durante un segundo y luego se `muestre`{:class="block3looks "}:

![](images/fly-icon.png)

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

**Prueba:** Ensaya que tu libélula ahora pueda comer muchas moscas.

Asegúrate de haber agregado el bloque `mostrar`{:class="block3looks"} para mostrar al principio.

--- /task ---

**Sugerencia:** Puedes pulsar en el botón rojo **Detener** sobre el escenario si deseas que la libélula permanezca parada mientras agregas más código.

--- save ---
