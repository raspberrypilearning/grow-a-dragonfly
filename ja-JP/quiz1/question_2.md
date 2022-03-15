
--- question ---
---
legend: 質問2/3
---

トンボがマウスポインターに`触れた`の{:class="block3sensing"}`ではない`{:class="block3operators"}ときだけ動くようにコードを書きましたね。

トンボが動くたびに音が鳴るようにするには、`音を鳴らす`{:class="block3sound"} ブロックはどこに置くべきでしょうか。

--- choices ---

- ( )

```blocks3
when flag clicked
forever
+start sound [Wings v]
if <not <touching [mouse-pointer v] ?> > then
point towards (mouse-pointer v)
move [5] steps
end
end
```

--- feedback ---

残念！、このコードでは`音を鳴らす`{:class="block3sound"} ブロックは `もし`{:class="block3control"} ブロックの外にあるので、トンボが動かなくても`ずっと`{:class="block3control"} ループが走る度に実行されることになるのです。

--- /feedback ---

- (x)

```blocks3
when flag clicked
forever
if <not <touching [mouse-pointer v] ?> > then
+start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

  --- feedback ---

正解です！ `音を鳴らす`{:class="block3sound"} ブロックを `もし`{:class="block3control"} ブロックの中に置くと、トンボが動いた時に再生されることになります。

  --- /feedback ---

- ( )


```blocks3
when flag clicked
forever
if <not <touching [mouse-pointer v] ?> > then
point towards (mouse-pointer v)
move [5] steps
end
+start sound [Wings v]
end
```

  --- feedback ---

残念！、このコードでは`音を鳴らす`{:class="block3sound"} ブロックは `もし`{:class="block3control"} ブロックの外にあるので、トンボが動かなくても`ずっと`{:class="block3control"} ループが走る度に実行されることになるのです。

  --- /feedback ---

--- /choices ---

--- /question ---
