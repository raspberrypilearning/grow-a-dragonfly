## Quick quiz

Answer the three questions. There are hints to guide you to the correct answer.

When you have answered each question, click on **Check my answer**.

Have fun!

--- question ---
---
legend: Pregunta 1 de 3
---

A project uses the **Crab** sprite and the **Jellyfish** sprite. The **Crab** sprite has this code:

![desc](images/crab-icon.png)

```blocks3
when flag clicked
if <not <touching color (#0000FF)?>> then
hide
end
```

What would need to happen for the **Crab** sprite to hide?

--- choices ---

- () El objeto **Crab** necesitaría tocar el **Jellyfish**

 --- feedback ---

 No, el bloque `si`{:class="block3control"} tiene una condición `Sensores`{:class="block3sensing"}, pero no utiliza el bloque `tocando Jellyfish`{:clase="block3sensing"}.

 --- /feedback ---

- (x) El objeto **Crab** no debería tocar el color azul

 --- feedback ---

Yes, the `not`{:class="block3operators"} operator means that the condition is true `if`{:class="block3control"} the **Crab** sprite is not `touching`{:class="block3sensing"} the colour blue.

 --- /feedback ---

- () El objeto **Crab** tendría que estar tocando el color azul

 --- feedback ---

 No del todo, mira de cerca el `operador`{:class="block3operators"} en la condición.

 --- /feedback ---

- ( ) El objeto **Crab** siempre se va a `esconder`{:class="block3looks"} `al presionar la bandera verde`{:class="block3events"}

 --- feedback ---

 No, hay un bloque `si`{:class="block3control"} en el código del objeto **Crab** por lo que solo se ocultará si se cumple la condición.

 --- /feedback ---

--- /choices ---

--- /question ---
