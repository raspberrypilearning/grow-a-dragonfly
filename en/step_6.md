## More food

Now you will give the Dragonfly a choice of insects.

--- task ---
Right-click on the Insect sprite under the Stage and duplicate it. 

![](images/duplicate-insect.png)

--- /task ---

It's helpful if this insect looks different to the fly.

--- task ---

Click on the 'Costumes' tab. 

You can either:
+ Use the Fill tool to change the colour of this insect
+ 'Paint' your own insect costume, or
+ Add another bug costume from Scratch.

--- /task ---

The Fly gets eaten even if it touches the Dragonfly's wing or tail. That doesn't work well when the Dragonfly gets big.

To fix this you can use the `touching color`{:class="block3sensing"} block so the fly only gets eaten if it is touches a particular colour on the Dragonfly.


--- task ---

Select the Dragonfly sprite and click on the 'Costumes' tab.

Use the fill tool to fill in the Dragonfly's mouth. We used purple:

![](images/dragonfly-mouth-colour.png)

--- /task ---

You need to check that the **Insect 2** sprite is touching the Dragonfly sprite `and`{:class="block3operators"} touching the colour of the Dragonfly's mouth.

--- task ---

Select 'Insect 2' and click on the 'Code' tab.

Drag a `and`{:class="block3operators"} block into the `if`{:class="block3control"}. The `<touching [Dragonfly v] ?>`{:class="block3sensing"} block will pop out:

```blocks3
when flag clicked
forever
move [3] steps // Not eaten
if on edge, bounce
+if <<> and <>> then
broadcast [food v]
hide
go to (random position v)
show
end
end
```

--- /task ---


--- task ---

Drag the `<touching [Dragonfly v] ?>`{:class="block3sensing"} into the left of the `and`{:class="block3operators"} block:

```blocks3
when flag clicked
forever
move [3] steps // Not eaten
if on edge, bounce
+if <<<touching [Dragonfly v] ?>> and <>> then
broadcast [food v]
hide
go to (random position v)
show
end
end
```

--- /task ---

--- task ---

Drag a `touching color`{:class="block3sensing"} block into the right of the `and`{:class="block3operators"} block:

```blocks3
when flag clicked
forever
move [3] steps // Not eaten
if on edge, bounce
+if <<touching [Dragonfly v] ?> and <touching color (#9966ff) ?>> then
broadcast [food v]
hide
go to (random position v)
show
end
end
```

If it doesn't have the colour of the Dragonfly's mouth selected then click on the colour and then click on the Eyedropper to select a colour.


![](images/colour-eyedropper.png)

Click on the Dragonfly's mouth on the Stage to set the colour to match:

![](images/colour-select.png)

**Tip:** If this is tricky to do, change the size of the Dragonfly so it's really big.

--- /task ---

--- task ---
**Test:** Now test that the Dragonfly can only eat the second insect with its mouth. 

If you like, you can change the first Insect so that it can only be eaten with the Dragonfly's mouth.

--- /task ---

--- save ---

