## Quick quiz

Answer the three questions. There are hints to guide you to the correct answer.

When you have answered each question, click on **Check my answer**.

Have fun!

--- question ---
---
legend: 質問1/3
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

- () **Crab** スプライトは **Jellyfish**に触れる必要があります

 --- feedback ---

 残念！、`もし`{:class="block3control"}ブロックには`調べる`{:class="block3sensing"}条件がありますが、`Jellyfishに触れた`{:class="block3sensing"} ブロックは使用されていません。

 --- /feedback ---

- (x) **Crab** スプライトは青色に触れていない必要があります。

 --- feedback ---

Yes, the `not`{:class="block3operators"} operator means that the condition is true `if`{:class="block3control"} the **Crab** sprite is not `touching`{:class="block3sensing"} the colour blue.

 --- /feedback ---

- () **Crab** スプライトは青色をふれる必要があります。

 --- feedback ---

 残念！、条件の中の`演算子`{:class="block3operators"}をよく見てみてください。

 --- /feedback ---

- ( ) `旗が押されたとき`{:class="block3events"}、**Crab**スプライトは常に`隠れる`{:class="block3looks"}ようになります。

 --- feedback ---

 残念！、`もし`{:class="block3control"}ブロックが**Crab**スプライトのコードにあり、条件が満たされたときだけ隠れるようになっています。

 --- /feedback ---

--- /choices ---

--- /question ---
