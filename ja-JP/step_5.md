## 動きの改善

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
マウスポインターがトンボに触れてしまうと、トンボは壊れたよう機械の用に激しく方向を変え続けます。 これを修正するには、別の条件を確認する必要があります。
</div>
<div>
![昆虫とトンボが映し出されるステージ。](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

**Dragonfly**を選択し、`「緑の旗」が押されたとき`{:class="block3events"}で始まるスクリプトを見つけます。

`ずっと`{:class="block3control"}ブロックの中に`もし`{:class="block3control"}をドラッグすると、`ずっと`{:class="block3control"}の中のブロックは`もし`{:class="block3control"}の中に移動します。

コードが次のようになっていることを注意深く確認してください。

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if < > then
start sound [羽音 v]
point towards (mouse-pointer v)
move [5] steps
end
end
```
--- /task ---

--- task ---

そして、`ではない`{:class="block3operators"}ブロックを`もし`{:class="block3control"}に、`(マウスポインター)に触れた`{:class="block3sensing"} をその中にドラッグしてください。

以下のようなコードになっているか確認してください。

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if <not <touching [mouse-pointer v] ?> > then
start sound [羽音 v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

`ではない`{:class="block3operators"} ブロックは、文章と同じように、条件をその反対に変えます。

--- /task ---

--- task ---

**テスト:**不具合が修正され、トンボが`(マウスポインター)に触れた`{:class="block3sensing"}の`ではない`{:class="block3operators"}ときにのみ動くことを確認します。

別の条件で試してみる場合は：

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

これにより、マウスポインターから十分に離れているときに、トンボが移動します。

**ヒント：** コード領域の任意の場所にブロックをドラッグして、さまざまなことを試す間、そこに置いたままにすることができます。

--- /task ---

--- save ---
