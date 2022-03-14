## シーンを設定する

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
シーンを設定します。 背景を選び、マウスポインターを追ってステージを回るトンボを追加します。
</div>
<div>
![](images/set-the-scene.png){:width="300px"}
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

![](images/choose-backdrop-icon.png)

![Jurassicの背景を使ったステージ。](images/Jurassic-backdrop.png)

--- /task ---

--- task ---

**スプライトを選ぶ**をクリックし、`dragonfly`を検索して、**Dragonfly**スプライトを追加します。

![](images/choose-sprite-icon.png)

![「dragonfly」と入力された検索ボックスと、ギャラリー内のDragonflyのスプライト。](images/dragonfly-search.png)

--- /task ---

--- task ---

**Dragonfly** スプライトをマウスポインタ(または指) に追従させるスクリプトを追加する。

![](images/dragonfly-icon.png)

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

Click on the **Costumes** tab and use the **Select** (arrow) tool to select the costume. Use the **Rotate** tool at bottom of the selected costume to turn the **Dragonfly** costume to face the right.

![An animated image showing how to rotate the dragonfly costume by dragging the rotation arrows so that the dragonfly faces right.](images/rotated-costume.gif)

![The dragonfly costume selected and turned to face the right.](images/rotated-costume.png)

--- /task ---

--- task ---

**Test:** Click the green flag and look at how the dragonfly moves now.

--- /task ---

Dragonfly wings make a fluttering sound as they vibrate. You can edit a sound in Scratch to create your own sound.

--- task ---

Add the **Crank** sound to the **Dragonfly** sprite.

[[[generic-scratch3-sound-from-library]]]

![](images/crank-sound-editor.png)

Click the **Play** button so you can hear the sound.

--- /task ---

The **Crank** sound is too long and too slow for dragonfly wings.

--- task ---

Select the end of the sound using your cursor or finger.

Click **Copy to New** to make a new sound with just the selected part:

![The end of the crank sound selected in blue with the 'Copy to New' icon highlighted.](images/crank-copy-end.png)

Rename your new sound from **Crank2** to `Wings`.

![The rename sound property.](images/crank-wings-sound.png)

--- /task ---

--- task ---

Play the new sound. Click the **Faster** button a few times until you like the result:

![A faster sound wave with the 'Faster' icon highlighted.](images/wings-faster.png)

--- /task ---

--- task ---

If you like, you can select the very end of the **Wings** sound, and then click **Delete** to remove it:

![The end of the sound wave selected with the 'Delete' tool highlighted.](images/wings-shorter.png)

--- /task ---

--- task ---

Now add a block to play the **Wings** sound when the dragonfly moves:

![](images/dragonfly-icon.png)

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

**Test:** Try out your dragonfly movement and sound effect.

--- /task ---

--- save ---
