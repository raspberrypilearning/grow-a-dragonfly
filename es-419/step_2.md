## Prepara la escena

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Prepararás la escena. Elige tu fondo y agrega una libélula que siga el puntero del ratón alrededor del escenario.
</div>
<div>
![Dragonfly in a desert background](images/set-the-scene.png){:width="300px"}
</div>
</div>

--- task ---

Abre el [proyecto inicial Haz crecer una libélula](https://scratch.mit.edu/projects/535695413/editor){:target="_blank"}. Scratch se abrirá en otra pestaña del navegador.

[[[working-offline]]]

--- /task ---

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
¡Las <span style="color: #0faeb0">**Libélulas**</span> se pueden encontrar en todo el mundo y han existido por más de 300 millones de años!</p>

--- task ---

**Elige:** Pulsa **Elige un Fondo** y agrega un fondo de tu elección. Hemos usado el fondo **Jurassic**.

![Backdrop icon on the Scratch app interface](images/choose-backdrop-icon.png)

![El Escenario que se muestra es el fondo Jurassic.](images/Jurassic-backdrop.png)

--- /task ---

--- task ---

Pulsa sobre **Elegir un Objeto** y busca `dragonfly`, luego agrega el objeto **Dragonfly**.

![Sprite icon on the Scratch app interface](images/choose-sprite-icon.png)

![El cuadro de búsqueda con 'dragonfly' escrito y el objeto Dragonfly en la galería.](images/dragonfly-search.png)

--- /task ---

--- task ---

Agrega un script para hacer que el **Dragonfly** siga el puntero del ratón (o tu dedo):

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

**Prueba:** Presiona la bandera verde y haz que el objeto **Dragonfly** se mueva por el Escenario. ¿Se está moviendo la libélula como era de esperar?

--- /task ---

El disfraz de Libélula no mira hacia la derecha, por lo que la cabeza del objeto **Dragonfly** no apunta hacia el puntero del ratón.

--- task ---

Pulsa en la pestaña **Disfraces** y usa la herramienta **Seleccionar** (flecha) para seleccionarlo. Utiliza la herramienta **Rotar** en la parte inferior del disfraz seleccionado para girar a **Dragonfly** y que mire hacia la derecha.

![Una imagen animada que muestra cómo rotar el disfraz de libélula arrastrando las flechas de rotación para que mire hacia la derecha.](images/rotated-costume.gif)

![El disfraz de libélula seleccionado y girado para que mire hacia la derecha.](images/rotated-costume.png)

--- /task ---

--- task ---

**Prueba:** Presiona la bandera verde y observa cómo se mueve ahora la libélula.

--- /task ---

Las alas de la libélula hacen un sonido de aleteo mientras vibran. Puedes editar un sonido en Scratch para crear el tuyo propio.

--- task ---

Agrega el sonido **Crank** al objeto **Dragonfly**.

[[[generic-scratch3-sound-from-library]]]

![](images/crank-sound-editor.png)

Pulsa en el botón **Reproducir** para que puedas escuchar el sonido.

--- /task ---

El sonido **Crank** es demasiado largo y demasiado lento para las alas de la libélula.

--- task ---

Selecciona el final del sonido con tu puntero del ratón o dedo.

Pulsa en **Copiar a uno nuevo** para crear un sonido nuevo sólo con la parte seleccionada:

![El final del sonido crank seleccionado en azul con el ícono 'Copiar a uno nuevo' resaltado.](images/crank-copy-end.png)

Cambia el nombre de tu nuevo sonido de **Crank2** a `Wings`.

![La propiedad de renombrar sonido.](images/crank-wings-sound.png)

--- /task ---

--- task ---

Reproduce el nuevo sonido. Pulsa en el botón **Más rápido** varias veces hasta que te guste el resultado:

![Una onda de sonido más rápida con el ícono 'Más rápido' resaltado.](images/wings-faster.png)

--- /task ---

--- task ---

Si quieres, puedes seleccionar el final del sonido **Wings**, y luego pulsar **Eliminar** para quitarlo:

![El final de la onda de sonido seleccionada con la herramienta 'Eliminar' resaltada.](images/wings-shorter.png)

--- /task ---

--- task ---

Ahora agrega un bloque para reproducir el sonido **Wings** cuando la libélula se mueva:

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

**Prueba:** Prueba el movimiento y efecto de sonido de tu libélula.

--- /task ---

--- save ---
