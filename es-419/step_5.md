## Movimiento mejorado

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
La libélula 'falla' y cambia de dirección muy rápido si el puntero del ratón está tocando la libélula. Comprobarás otra condición para arreglar esto.
</div>
<div>
![El escenario mostrando un insecto y una libélula.](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

Selecciona **Dragonfly** y busca el script que comienza con `al presionar la bandera`{:class="block3events"}.

Arrastra un `si`{:class="block3control"} dentro del bloque `por siempre`{:class="block3control"} y los bloques dentro del `por siempre`{:class="block3control"} se moverán dentro del `si`{:clase="bloque3control"}.

Comprueba cuidadosamente que tu código se vea así:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if < > then
start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
end
```
--- /task ---

--- task ---

Luego arrastra un bloque `no`{:class="block3operators"} dentro del `si`{:class="block3control"} y un `tocando (el puntero del ratón)`{:class="block3sensing"} dentro suyo.

Comprueba que tu código sea como esto:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if <not <touching [mouse-pointer v] ?> > then
start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

El bloque `no`{:class="block3operators"} convierte una condición en su opuesta, tal como lo haría en una frase.

--- /task ---

--- task ---

**Prueba:** Comprueba que el fallo está arreglado y que el Dragonfly solo se mueve cuando está `no`{:class="block3operators"} `tocando (puntero del ratón)`{:class="block3sensing"}.

Una condición diferente para probar es:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

Esto hace que la libélula se mueva cuando está lo suficientemente lejos del puntero del ratón.

**Sugerencia:** Puedes arrastrar bloques a cualquier parte del área de Código y dejarlos allí mientras intentas diferentes cosas.

--- /task ---

--- save ---
