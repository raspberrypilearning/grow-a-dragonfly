## Quiz rápido

Responda três perguntas. Há dicas para guiá-lo para a resposta correta.

Depois de responder a cada pergunta, clique em **Verificar resposta**.

Divirta-se!

--- question ---
---
legenda: Pergunta 1 de 3
---

Um projeto usa o sprite **Crab** e o sprite **Jellyfish**. O sprite **Crab** tem este código:

![descrição](images/crab-icon.png)

```blocks3
when flag clicked
if <not <touching color (#0000FF)?>> then
hide
end
```

O que precisaria acontecer para o sprite **Crab** se esconder?

--- choices ---

- () O sprite **Crab** precisaria tocar o **Jellyfish**

 --- feedback ---

 Não, o bloco `if`{:class="block3control"} tem uma condição `Sensing`{:class="block3sensing"}, mas não usa o bloco `touching Jellyfish`{:class="block3sensing"}.

 --- /feedback ---

- (x) O sprite **Crab** precisaria não tocar na cor azul

 --- feedback ---

Sim, o operador `not`{:class="block3operators"} significa que a condição é verdadeira `if`{:class="block3control"} o sprite **Crab** não é `tocando`{:class="block3sensing"} a cor azul.

 --- /feedback ---

- () O sprite **Crab** precisaria estar tocando a cor azul

 --- feedback ---

 Não exatamente, observe atentamente o `operator`{:class="block3operators"} na condição.

 --- /feedback ---

- ( ) O sprite **Crab** sempre `esconderá`{:class="block3looks"} `quando o sinalizador for clicado`{:class="block3events"}

 --- feedback ---

 Não, há um bloco `if`{:class="block3control"} no código do sprite **Crab** , então ele só será ocultado se a condição for atendida.

 --- /feedback ---

--- /choices ---

--- /question ---
