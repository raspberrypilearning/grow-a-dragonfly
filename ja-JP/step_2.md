## シーンを設定する

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
シーンを設定します。 背景を選び、マウスポインターを追ってステージを回るトンボを追加します。
</div>
<div>
![Dragonfly in a desert background](images/set-the-scene.png){:width="300px"}
</div>
</div>

--- task ---

[成長するトンボスタータープロジェクト](https://scratch.mit.edu/projects/535695413/editor){:target="_blank"}を開きます。 スクラッチはブラウザの別のタブで開きます。

[[[working-offline]]]

--- /task ---

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">**トンボ***</span>は世界中に生息しており、3億年以上前から生息しているそうです</p>

--- task ---

**選択：****背景を選ぶ**をクリックし、お好みの背景を追加します。 **Jurassic** の背景を使用しました。

![Backdrop icon on the Scratch app interface](images/choose-backdrop-icon.png)

![Jurassicの背景を使ったステージ。](images/Jurassic-backdrop.png)

--- /task ---

--- task ---

**スプライトを選ぶ**をクリックし、`dragonfly`を検索して、**Dragonfly**スプライトを追加します。

![Sprite icon on the Scratch app interface](images/choose-sprite-icon.png)

![「dragonfly」と入力された検索ボックスと、ギャラリー内のDragonflyのスプライト。](images/dragonfly-search.png)

--- /task ---

--- task ---

**Dragonfly** スプライトをマウスポインタ(または指) に追従させるスクリプトを追加する。

![Dragonfly sprite icon on the Scratch app interface](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] % // to start small
forever
point towards (mouse-pointer v)
move [5] steps
end
```
--- /task ---

--- task ---

**テスト：** 緑の旗をクリックし、**Dragonfly**のスプライトをステージ上で移動させます。 トンボは期待通りに動いていますか？

--- /task ---

トンボの衣装は右向きではないので、**Dragonfly**スプライトの頭はマウスポインタの方に向いていません。

--- task ---

**コスチューム**タブをクリックし、**選択**(矢印) ツールでコスチュームを選択します。 選択したコスチュームの下にある**回転**ツールを使って、**Dragonfly**コスチュームを右向きにします。

![トンボのコスチュームが右を向くように回転矢印をドラッグして回転させる様子を示すアニメーション画像。](images/rotated-costume.gif)

![選択され、右を向いたトンボのコスチューム。](images/rotated-costume.png)

--- /task ---

--- task ---

**テスト：**緑の旗をクリックして、トンボの動きを見てください。

--- /task ---

トンボの羽は、振動するとヒラヒラと音がします。 Scratchで音を編集して、自分だけの音を作ることができます。

--- task ---

**Dragonfly** スプライトに**クランク**サウンドを追加します。

[[[generic-scratch3-sound-from-library]]]

![](images/crank-sound-editor.png)

**再生**ボタンをクリックすると、音が出ます。

--- /task ---

**クランク** の音は、トンボの羽音には長すぎて遅すぎます。

--- task ---

カーソルまたは指で音の終わりの部分を選択します。

**音をコピー**をクリックすると、選択した部分だけを使った新しいサウンドが作成されます。

![クランク音の末尾が青く選択され、「音をコピー」アイコンが強調表示されます。](images/crank-copy-end.png)

新しいサウンドの名前を**Crank2**から`羽音`に変更します。

![サウンドの名前の変更プロパティ。](images/crank-wings-sound.png)

--- /task ---

--- task ---

新しいサウンドを再生します。 気に入った結果が得られるまで、**速く**ボタンを数回クリックしてください。

![「速く」のアイコンが強調表示された、より速い波形。](images/wings-faster.png)

--- /task ---

--- task ---

お好みで、**羽音**の音の最後の部分を選択し、**削除**をクリックして削除することもできます。

![波形の最後の部分が選択された波形と強調表示された「削除」ツール。](images/wings-shorter.png)

--- /task ---

--- task ---

次に、トンボが動いたときに**羽音**という音を鳴らすブロックを追加します。

![Dragonfly sprite icon](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
```
--- /task ---

--- task ---

**テスト：** トンボの動きと効果音を試してみる。

--- /task ---

--- save ---
