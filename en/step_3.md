## A fly to eat

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
In this step, you will add an insect for the Dragonfly to eat. 
</div>
<div>
![](images/fly-to-eat.png){:width="300px"}
</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
Characters that move around on their own in games are sometimes called <span style="color: #0faeb0">**mobs**</span>, short for mobile. Can you think of a game that has mobs?</p>

There's a fly in the 'Frog 2' sprite that you can use.

![](images/frog-sprite.png)

--- task ---

Add the 'Frog 2' sprite to your project. Rename the sprite to 'Insect':

![](images/fly-sprite.png)


--- /task ---

You only need the fly, not the Frog.

--- task ---
Click on the **Costumes** tab. Click on the fly to select it and click on the **Copy** icon.

![](images/copy-fly.png)

--- /task ---

--- task ---
Add a new costume to the sprite using the 'Paint' option:

![](images/paint-sprite.png)

--- /task ---

--- task ---
Click on the **Paste** icon to paste the sprite into the new costume. Drag the fly to the **center** so it lines up with the crosshair.

You can rename your costume 'Insect' and delete the other costumes as you won't need those:

![](images/fly-costume.png)

--- /task ---

--- task ---

Increase the size of the fly so that it's easier to see and catch:

![Size property set to 150](images/fly-size.png)

--- /task ---

--- task ---

Click on the **Code** tab and add a script to make the **Insect** sprite bounce around:

![](images/fly-icon.png)

```blocks3
when flag clicked
forever
move [3] steps
if on edge, bounce
end
```

The `if on edge, bounce`{:class="block3motion"} block checks to see if the sprite has reached the edge of the Stage and points the sprite in a different direction if it has. 

--- /task ---

You want the **Insect** sprite to `hide`{:class="block3looks"} `if`{:class="block3control"} it gets eaten by the **Dragonfly** sprite. 

--- task ---

Add an `if`{:class="block3control"} block to the Insect's movement script:

![](images/fly-icon.png)

```blocks3
when flag clicked
forever
move [3] steps
if on edge, bounce
+if < > then 
end
```
--- /task ---

The `if`{:class="block3control"} has a hexagon-shaped input. This means you can put a **condition** here. When the `if`{:class="block3control"} block runs, Scratch will check the condition, `if`{:class="block3control"} the condition is 'true' `then`{:class="block3control"} the code inside the `if`{:class="block3control"} block will run.

You want the Insect to `hide`{:class="block3looks"} `if`{:class="block3control"} it is `touching`{:class="block3sensing"} the **Dragonfly** sprite.

--- task ---

Drag a `touching [Dragonfly v]`{:class="block3sensing"} into the `if`{:class="block3control"} block. Add a `hide`{:class="block3looks"} block inside the `if`{:class="block3control"} block.

![](images/fly-icon.png)

```blocks3
when flag clicked
forever
move [3] steps
if on edge, bounce
+if <touching [Dragonfly v] ?> then // change from 'mouse-pointer'
+hide 
end
```

--- /task ---

--- task ---

**Test:** Test your code and control the Dragonfly to eat the fly. The fly should disappear.

--- /task ---

The Dragonfly won't get very big if it can only eat one fly! 

--- task ---

Add blocks to go to a random position on the Stage and make your sprite `wait`{:class="block3control"} for one second then show:

![](images/fly-icon.png)

```blocks3
when flag clicked
+show // show at the start
forever
move [3] steps
if on edge, bounce
if <touching [Dragonfly v] ?> then
hide
+go to (random position v)
+wait [1] seconds
+show
end
end
```

--- /task ---

--- task ---

**Test:** Test that your Dragonfly can now eat lots of flies.

Make sure you have added the `show`{:class="block3looks"} block to show at the start.

--- /task ---

**Tip:** You can click the red 'Stop' button above the Stage if you want the dragonfly to be quiet while you add more code.

--- save ---