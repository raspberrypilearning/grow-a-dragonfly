## ふりかえり

よくできました。ユーザーが制御するトンボと、アルゴリズムに従う昆虫を使って、ネイチャーアプリを作成しました。

`イベント`{:class="block3events"}、 `制御`{:class="block3control"}、 `調べる`{:class="block3sensing"}、`演算`{:class="block3operators"}、`動き`{:class="block3motion"}、 `見た目`{:class="block3looks"}および `音`{:class="block3sound"}ブロックを使用しました！

次はふりかえりの時間です。ふりかえりを行うことで、脳に新しいつながりを作ることができます。このため、ふりかえりは学習の大事な部分です。

以下の3つの質問に答えて、学んだことをふりかえってみましょう。

各質問の後で、送信を押します。 正しい答えが表示されます。 このアクティビティは何度でも実行できます。

楽しんで!

--- question ---
---
legend: 質問1/3
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

正解！、`ではない`{:class="block3operators"}演算子は、`もし`{:class="block3control"}**Crab**スプライトが青色に`触れている`{:class="block3sensing"}ではない、という条件が真であることを意味します。

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
