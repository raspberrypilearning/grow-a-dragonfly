## Random insect movement

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
The insects move in a very predictable pattern. 

Use the `pick random`{:class="block3operators"} block to make the insect move in a more natural way.

</div>
<div>
![Stage showing insects pointing in different directions.](images/random-movement.png){:width="300px"}
</div>
</div>

--- task ---

Add a script to **Insect 2** to make it point in a random direction every 1–3 seconds. 

![](images/insect2-icon.png)

```blocks3
when flag clicked
forever // Keep changing direction
point in direction (pick random [0] to [259])
wait (pick random [1] to [3]) seconds
end
```

--- /task ---

--- task ---

**Test:** Run your project and watch how the sprite moves. 

--- /task ---

--- task ---

Drag this script to the other **Insect** sprite to make it move randomly.

--- /task ---

--- task ---

Change the number of steps the sprites `move`{:class="block3motion"} to make them faster or slower.

--- /task ---

--- save ---
