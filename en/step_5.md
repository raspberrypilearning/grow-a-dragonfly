## Improved movement

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
In this step, you will improve the Dragonfly's movement. Have you noticed that the Dragonfly 'glitches' and changes direction really fast if the mouse pointer is touching the Dragonfly?
</div>
<div>
![](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

Select the Dragonfly and find the script that starts with `when flag clicked`{:class="block3events"}.

Drag an `if`{:class="block3control"} inside the `forever`{:class="block3control"} block and the blocks inside the `forever`{:class="block3control"} will move inside the `if`{:class="block3control"}.

Check carefully that your code looks like this:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if < > then
start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
end
```
--- /task ---

--- task ---

Then drag a `not`{:class="block3operators"} block into the `if`{:class="block3control"} and a `touching (mouse-pointer)`{:class="block3sensing"} inside that.

Check that your code looks like this:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if <not <touching [mouse-pointer v] ?> > then
start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

The `not`{:class="block3operators"} block turns a condition into its opposite, just like it would in a sentence. 

--- /task ---

--- task ---
**Test:** Check that the glitch is fixed and the Dragonfly only moves when it is `not`{:class="block3operators"} `touching (mouse-pointer)`{:class="block3sensing"}.

A different condition to try is:

```blocks3
<(distance to [mouse-pointer v]) > [50]>
```

This makes the Dragonfly move when it's far enough from the mouse pointer. Try it and see which you prefer.

**Tip:** You can drag blocks anywhere in the Code area and leave them there while you try different things. If you prefer what you had earlier you can easily put it back.

--- /task ---

--- save ---