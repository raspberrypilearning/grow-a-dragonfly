## Quick quiz

Answer the three questions. 正しい答えが表示されます。

When you have answered each question, click on **Check my answer**.

楽しんで!

--- question ---
---
legend: Question 1 of 3
---

あるプロジェクトで**Crab**スプライトと**Jellyfish**スプライトが使用されています。 **Crab**スプライトは、このようなコードを持っています。

![desc](images/crab-icon.png)

```blocks3
when flag clicked
if <not <touching color (#0000FF)?>> then
hide
end
```

**Crab**のスプライトが隠れるには何が必要ですか？

--- choices ---

- () **Crab** スプライトは **Jellyfish**に触れる必要があります

 --- feedback ---

 残念！、`もし`{:class="block3control"}ブロックには`調べる`{:class="block3sensing"}条件がありますが、`Jellyfishに触れた`{:class="block3sensing"} ブロックは使用されていません。

 --- /feedback ---

- (x) **Crab** スプライトは青色に触れていない必要があります。

 --- feedback ---

正解！ 、`ではない`{:class="block3operators"}演算子は、`もし`{:class="block3control"}**Crab**スプライトが青色に`触れている`{:class="block3sensing"}ではない、という条件が真であることを意味します。

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
