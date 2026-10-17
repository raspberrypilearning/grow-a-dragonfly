## Más comida

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
La libélula necesita una selección de insectos.
</div>
<div>
![Escenario con dos insectos y la libélula.](images/more-food.png){:width="300px"}
</div>
</div>

--- task ---

Pulsa con el botón derecho en el objeto **Insecto** en la lista de Objetos debajo del Escenario y selecciona **duplicar**.

![La lista de Objetos con el objeto insecto seleccionado y 'duplicar' resaltado en el menú.](images/duplicate-insect.png)

--- /task ---

Make this insect look different to the fly.

--- task ---

Click on the **Costumes** tab and create a different flying insect.

+ Use the **Fill** tool to change the colour of this insect.
+ **Paint** your own insect costume.
+ **Add** another bug costume from Scratch.

--- /task ---

El insecto será comido incluso si toca el ala o la cola de la libélula.

Para que tu app sea más realista, arregla esto para que al insecto lo coman por la boca de la libélula. Puedes usar el bloque `tocando el color`{:class="block3sensing"} para que solo lo coman si toca un color en particular en el **Dragonfly**.

--- task ---

Selecciona el objeto **Dragonfly** y pulsa en la pestaña **Disfraces**.

Utiliza la herramienta de relleno para rellenar la boca del **Dragonfly**. Nosotros hemos usado morado:

![El editor de Pintura con la herramienta Relleno seleccionada y el disfraz de libélula con la boca morada.](images/dragonfly-mouth-colour.png)

--- /task ---

You need to check that the new sprite is touching the **Dragonfly** sprite `and`{:class="block3operators"} touching the colour of the dragonfly's mouth.

--- task ---

Select your new sprite and click on the **Code** tab.

Arrastra un bloque `y`{:class="block3operators"} dentro del bloque `si`{:class="block3control"}.

The `<touching [Dragonfly v] ?>`{:class="block3sensing"} block will pop out, drag it into a space in the `and`{:class="block3operators"} block:

![](images/insect2-icon.png)

```blocks3
when flag clicked
show
forever
move [3] steps 
if on edge, bounce
+if <<touching [Dragonfly v] ?> and <>> then
broadcast [food v]
hide
go to (random position v)
show
end
end
```

--- /task ---

--- task ---

Drag a `touching color`{:class="block3sensing"} block into the other space of the `and`{:class="block3operators"} block:

```blocks3
when flag clicked
show
forever
move [3] steps
if on edge, bounce
+if <<touching [Dragonfly v] ?> and <touching color (#9966ff) ?>> then
broadcast [food v]
hide
go to (random position v)
show
end
end
```

If it doesn't have the colour of the dragonfly's mouth selected, click on the colour circle and then click on the **Eyedropper** tool at the bottom to select a colour.

![El menú del círculo de colores con la herramienta cuentagotas.](images/colour-eyedropper.png)

Click on the dragonfly's mouth on the Stage to set the colour:

![La herramienta cuentagotas con resaltador de selección de color flotando sobre la boca púrpura de la libélula.](images/colour-select.png)

**Tip:** If the small mouth is hard to select, make the **Dragonfly** sprite bigger.

--- /task ---

--- task ---

**Test:** Check the dragonfly can only eat the second insect with its mouth.

--- /task ---

--- save ---

