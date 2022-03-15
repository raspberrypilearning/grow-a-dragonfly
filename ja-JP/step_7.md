## ランダムな昆虫の動き

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
アプリの中の昆虫は非常に予測しやすい動きをしていますが、現実にはなかなか捕まえられないものです。 

昆虫の動きをより自然にするために、`乱数`{:class="block3operators"} ブロックを使用することになります。
</div>
<div>
![昆虫が様々な方向を向いているステージ。](images/random-movement.png){:width="300px"}
</div>
</div>

--- task ---

**昆虫2**にスクリプトを追加し、1〜3秒ごとにランダムな方向を向くようにします。

```blocks3
when flag clicked
forever // Keep changing direction
point in direction (pick random [0] to [259])
wait (pick random [1] to [3]) seconds
end
```

--- /task ---

--- task ---

**テスト：** プロジェクトを実行し、ハエの動きを見てみましょう。 必要な効果を得るために数値を変更してみてください。

また、このスクリプトを**昆虫**スプライトにドラッグすると、そちらもランダムに動くようになります。

--- /task ---

--- task ---

昆虫が思い通りの動きをするようになるまで、変えてみてください。

`動かす`{:class="block3motion"}のステップ数を変えて、速くしたり遅くしたりできます。

トンボの速度を変更することもできます。

--- /task ---

--- task ---

トンボがフルサイズに達するまで成長するのに必要なサイズを変更することもできます。

プロジェクトに満足するまで変更を加えます。

--- /task ---

--- save ---
