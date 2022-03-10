## Mouvement aléatoire des insectes

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Les insectes de ton application se déplacent selon un schéma très prévisible, mais dans la vraie vie, ils sont difficiles à attraper. 

Tu utiliseras le bloc « nombre aléatoire »{:class="block3operators"} pour faire bouger l'insecte de manière plus naturelle.
</div>
<div>
![Scène montrant des insectes pointant dans différentes directions.](images/random-movement.png){:width="300px"}
</div>
</div>

--- task ---

Ajoute un script à **Insecte2** pour le faire pointer dans une direction aléatoire toutes les 1 à 3 secondes.

```blocks3
when flag clicked
forever // Continue à changer de direction
point in direction (pick random [0] to [259])
wait (pick random [1] to [3]) seconds
end
```

--- /task ---

--- task ---

**Test :** Exécute ton projet et observe le mouvement de la mouche. Essaie de changer les nombres pour obtenir l'effet souhaité.

Tu peux également faire glisser ce script vers le sprite **Insecte** afin qu'il se déplace également de manière aléatoire.

--- /task ---

--- task ---

Modifie les insectes jusqu'à ce qu'ils se comportent comme tu le souhaites.

Tu peux modifier le nombre de pas qu'ils `font`{:class="block3motion"} pour les rendre plus rapides ou plus lents.

Tu peux également modifier la vitesse de la libellule.

--- /task ---

--- task ---

Tu peux également modifier la taille dont la libellule a besoin pour atteindre sa taille maximale.

Apporte des modifications jusqu'à ce que tu sois satisfait de ton projet.

--- /task ---

--- save ---
