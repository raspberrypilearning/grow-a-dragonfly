## Movimiento aleatorio de insectos

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Los insectos en tu aplicación se mueven en un patrón muy predecible, pero en la vida real son difíciles de atrapar. 

Usarás el bloque `elegir número al azar`{:class="block3operators"} para hacer que el insecto se mueva de una forma más natural.
</div>
<div>
![Escenario que muestra insectos apuntando en diferentes direcciones.](images/random-movement.png){:width="300px"}
</div>
</div>

--- task ---

Agrega un script al **Insect 2** para hacer que apunte en una dirección aleatoria cada 1-3 segundos.

```blocks3
when flag clicked
forever // Sigue cambiando de dirección
point in direction (pick random [0] to [259])
wait (pick random [1] to [3]) seconds
end
```

--- /task ---

--- task ---

**Prueba:** Ejecuta tu proyecto y observa cómo se mueve la mosca. Intenta cambiar los números para obtener el efecto que quieres.

También puedes arrastrar este script al objeto **Insecto** para que también se mueva aleatoriamente.

--- /task ---

--- task ---

Cambia los insectos hasta que se comporten como tú quieras.

Puedes cambiar la cantidad de pasos que se `mueven`{:class="block3motion"} para hacerlos más rápidos o más lentos.

También puedes cambiar la velocidad de la libélula.

--- /task ---

--- task ---

También puedes cambiar el tamaño que la libélula necesita crecer para alcanzar su tamaño completo.

Realiza cambios hasta que estés conforme con tu proyecto.

--- /task ---

--- save ---
