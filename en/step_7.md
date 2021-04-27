## Random insect movement

The insects move in a very predictable pattern. The `pick random`{:class="block3operators"} block choose a number between a minimum and a maximum. You can use this to make the insect move in a more natural way.

--- task ---

Add a script to **Insect 2** to make it point in a random direction every 1-3 seconds. 

```blocks3
when flag clicked
forever // Keep changing direction
point in direction (pick random [0] to [259])
wait (pick random [1] to [3]) seconds
end
```

--- /task ---

--- task ---
**Test:** Run your project and watch how the fly moves. Try changing the numbers to get the effect you want. 

You can also drag this script to the **Insect** sprite so that it moves randomly.

--- /task ---

--- task ---
Change the insects until they behave the way you want them to. 

You could change the number of steps they `move`{:class="block3motion"} to make them faster or slower.

You could also change the speed of the Dragonfly. 

--- /task ---

--- task ---
You could also change the size that the Dragonfly needs to grow to reach full size.

Make changes until you are happy with your project.

--- /task ---

--- save ---