## Improved movement

Have you noticed that the Dragonfly 'glitches' and changes direction really fast if the mouse pointer is touching the Dragonfly?

You can use a `not`{:class="block3operators"} block with `touching (mouse-pointer)`{:class="block3sensing"} to fix this. The `not`{:class="block3operators"} block turns a condition into it's opposite, just like it would in a sentence. 

--- task ---

Select the Dragonfly and find the script that starts with `when flag clicked`{:class="block3events"}.

Add an `if`{:class="block3control"} inside the `forever`{:class="block3control"}. Drag it under the `forever`{:class="block3control"} block and the blocks inside the `forever`{:class="block3events"} will move inside the `if`{:class="block3control"}.

Check carefully that your code looks like this:

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
