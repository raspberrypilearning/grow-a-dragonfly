## Faire grandir jusqu'à sa taille maximale

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Tu feras grandir la libellule lorsqu'elle mange une mouche, et tu t'arrêteras si elle atteint sa taille maximale.
</div>
<div>
![La libellule de taille maximale sur la scène disant "J'ai atteint ma taille maximale !".](images/grow-to-fullsize.png){:width="300px"}
</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
Les plus grandes libellules vivantes se trouvent en Amérique centrale et ont une envergure de 19 cm (un peu plus grande que ta main). Le plus grand insecte jamais connu était le <span style="color: #0faeb0">**Meganeuropsis permiana**</span>, une libellule d'une envergure d'environ 75 cm (la taille d'une grande empreinte de pied).</p>

La mouche sait qu'elle a été mangée, et maintenant la libellule a besoin de le savoir pour qu'elle grandisse.

Lorsque tu dois faire savoir à un autre sprite que quelque chose s'est passé, tu peux utiliser un bloc `envoyer à tous`{:class="block3events"} comme tu l'as fait dans [Lancer des sorts](https://projects.raspberrypi.org/en/projects/broadcasting-spells){:target="_blank"}.

--- task ---

Ajoute un bloc `envoyer à tous`{:class="block3events"} au sprite **Insecte** avec un nouveau message `nourriture`{:class="block3events"} :

![](images/fly-icon.png)

```blocks3
when flag clicked
show // show at the start
forever
move [3] steps
if on edge, bounce
if <touching [Dragonfly v] ?> then
+broadcast [food v]
hide
go to (random position v)
wait [1] seconds
show
end
end
```
--- /task ---

Le sprite **Libellule** doit grandir lorsqu'il reçoit le message `nourriture`{:class="block3events"}.

--- task ---

Sélectionne le sprite **Libellule** et ajoute ce script :

![](images/dragonfly-icon.png)

```blocks3 
when I receive [food v]
change size by [5]
```

--- /task ---

--- task ---

Ajoute le son **Chomp** à la libellule et `joue-le`{:class="block3sound"} lorsqu'un insecte se fait manger :

![](images/dragonfly-icon.png)

```blocks3 
when I receive [food v]
+start sound [Chomp v]
change size by [5]
```
--- /task ---

--- task ---

**Test :** Exécute ton projet pour tester que la libellule grandit et fait un bruit de mastication lorsqu'elle mange une mouche.

--- /task ---

Lorsque la libellule atteint sa taille maximale, le jeu te félicite et s'arrête.

--- task ---

Ajoute un bloc `si`{:class="block3control"}.

La libellule a atteint sa taille maximale lorsque la `taille`{:class="block3looks"} `=`{:class="block3operators"} `100%`. Ajoute d'abord un opérateur `=`{:class="block3operators"} dans l'entrée en forme hexagonale :

![](images/dragonfly-icon.png)

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
+if <[ ] = [ ]> then
end
```
--- /task ---

--- task ---

Termine la construction de la condition en ajoutant une variable intégrée `taille`{:class="block3looks"} et saisis la valeur `100` :

![](images/dragonfly-icon.png)

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
+if <(size) = [100]> then
end
```
--- /task ---

--- task ---

Ajoute des blocs de sorte que `si`{:class="block3control"} la condition est vraie `alors`{:class="block3control"} la libellule `enverra à tous`{:class="block3events"} un message de fin et `dira`{:class="block3looks"} `J'ai atteint ma taille maximale !`

Enfin, ajoute un bloc `arrêter tout`{:class="block3control"} pour arrêter les autres scripts libellule :

![](images/dragonfly-icon.png)

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
if <(size) = [100]> then
+broadcast [end v]
+say [I got to full size!]
+stop [other scripts in sprite v] // change from 'all'
end
```
--- /task ---

--- task ---

Pour le moment, la mouche bouge toujours après la fin du projet. Ajoute ce script au sprite **Insecte**.

![](images/fly-icon.png)

```blocks3
when I receive [end v]
stop [other scripts in sprite v]
```

--- /task ---

--- task ---

**Test :** Clique sur le drapeau vert et continue à manger des mouches jusqu'à ce que ta libellule atteigne sa taille maximale.

--- /task ---

--- save ---
