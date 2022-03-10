
--- question ---
---
legend: Pregunta 2 de 3
---

Escribiste código para hacer que la libélula se mueva solo si `no`{:class="block3operators"} está `tocando`{:class="block3sensing"} el puntero del ratón.

¿Dónde pondrías un bloque `iniciar sonido`{:class="block3sound"} para hacer que la libélula emita un sonido cada vez que se mueve?

--- choices ---

- ( )

```blocks3
when flag clicked
forever
+start sound [Alas v]
if <not <touching [mouse-pointer v] ?> > then
point towards (mouse-pointer v)
move [5] steps
end
end
```

--- feedback ---

No, con este código el bloque `iniciar sonido`{:class="block3sound"} está fuera del bloque `si`{:class="block3control"}, por lo que se ejecutará cada vez que el ciclo `por siempre`{:class="block3control"} se ejecute, incluso si la libélula no se mueve.

--- /feedback ---

- (x)

```blocks3
when flag clicked
forever
if <not <touching [mouse-pointer v] ?> > then
+start sound [Alas v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

  --- feedback ---

Sí, eso es correcto. Colocando el bloque `iniciar sonido`{:class="block3sound"} dentro del bloque `si`{:class="block3control"} significa que se reproducirá cuando la libélula se mueva.

  --- /feedback ---

- ( )


```blocks3
when flag clicked
forever
if <not <touching [mouse-pointer v] ?> > then
point towards (mouse-pointer v)
move [5] steps
end
+start sound [Alas v]
end
```

  --- feedback ---

No, el bloque `iniciar sonido`{:class="block3sound"} está fuera del bloque `si`{:class="block3control"}, por lo que se ejecutará cada vez que el ciclo `por siempre`{:class="block3control"} se ejecute, incluso si la libélula no se mueve.

  --- /feedback ---

--- /choices ---

--- /question ---
