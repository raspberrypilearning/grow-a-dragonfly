## Défi

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Modifie le comportement de tes insectes et ajoutes-en davantage.
</div>
<div>
![Scène montrant trois types d'insectes différents et la libellule.](images/random-movement.png){:width="300px"}
</div>
</div>


--- task ---

Modifie la vitesse de la libellule.

--- /task ---

--- task ---

Modifie la taille que la libellule doit atteindre pour atteindre sa taille adulte.

--- /task ---

--- task ---

Modifie le premier **Insecte** afin qu'il ne puisse être mangé qu'avec la bouche de la libellule.

--- /task ---

### Ajouter plus d'insectes

Tu peux peindre tes propres insectes ou essayer d'ajouter un emoji moustique !

--- task ---

Utilise le clavier emoji pour ajouter un sprite **Emoji moustique**.

Duplique un sprite **insecte** existant puis clique sur l'onglet **Costumes**. **Peins** un nouveau costume et sélectionne l'outil **Texte**. Au lieu de saisir du texte, utilise le raccourci clavier emoji pour ton système d'exploitation :

- Windows - <kbd>⊞ Win</kbd> + <kbd>.</kbd>
- MacOS - <kbd>contrôle</kbd> + <kbd>commande</kbd> + <kbd>espace</kbd>
- Linux - <kbd>ctrl</kbd> + <kbd>.</kbd>

![Le clavier emoji contextuel avec la catégorie "animaux et nature" sélectionnée.](images/emoji-keyboard.png)

Sélectionne l'emoji **Moustique** pour l'insérer dans l'éditeur de peinture. Utilise l'outil **Sélectionner** (flèche) pour centrer, redimensionner et faire pivoter ton moustique jusqu'à ce que tu en sois satisfait.

![L'emoji moustique dans l'éditeur de peinture.](images/emoji-mosquito.png)

**Astuce :** les emojis peuvent avoir un aspect différent sur différents ordinateurs, ils peuvent donc ne pas être identiques sur une tablette et sur un ordinateur de bureau. Certains emojis ne sont pas disponibles sur certains ordinateurs, mais la plupart des ordinateurs modernes les prendront en charge.

--- /task ---

### Créer un mouvement aléatoire

Utilise le bloc `nombre aléatoire`{:class="block3operators"} pour que l'insecte se déplace de manière plus naturelle.

![Scène montrant des insectes pointant dans différentes directions.](images/random-movement.png){:width="300px"}

--- task ---

Ajoute un script à **Insecte2** pour le faire pointer dans une direction aléatoire toutes les 1 à 3 secondes.

![](images/insect2-icon.png)

```blocks3
when flag clicked
forever // Continue à changer de direction
point in direction (pick random [0] to [259])
wait (pick random [1] to [3]) seconds
end
```

--- /task ---

--- task ---

**Test :** exécute ton projet et observe le mouvement du sprite.

--- /task ---

--- task ---

Fais glisser ce script vers l'autre sprite **Insecte** afin qu'il se déplace de manière aléatoire.

--- /task ---

### Partager tes insectes

--- task ---

Utilise ton sac à dos pour échanger des insectes avec tes amis grâce à leurs projets « Faire grandir une libellule ».

Envoie le lien de ton projet à ton ami·e qui pourra y accéder, clique sur Sac à dos (celui situé sous l'espace de code) et glisse-dépose le sprite.

[[[scratch-backpack]]]

--- /task ---

--- task ---

Vérifie que chaque sprite et costume possède un nom qui décrit l'image. Cela rend ton projet plus facile à comprendre si tu y reviens plus tard.

--- /task ---

--- task ---

Fais un clic droit sur la zone Code et choisis **Nettoyer les blocs** pour que Scratch nettoie ton code.

--- /task ---

--- save ---
