## Ustawić scenę

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Ustawisz scenę. Wybierz tło i dodaj ważkę, która podąża za wskaźnikiem myszy na scenie.
</div>
<div>
![Ważka na pustynnym tle](images/set-the-scene.png){:width="300px"}
</div>
</div>

--- task ---

Otwórz [projekt startowy Wyhoduj ważkę ](https://scratch.mit.edu/projects/535695413/editor){:target="_blank"}. Scratch will open a blank project in a new browser tab.

--- /task ---

--- task ---

Click **Choose a Backdrop** and add a backdrop of your choice. Użyliśmy tła **Jurassic**.

![Ikona tła w interfejsie aplikacji Scratch](images/choose-backdrop-icon.png)

![Scena ukazująca jurajskie tło.](images/Jurassic-backdrop.png)

--- /task ---

--- task ---

Kliknij **Wybierz duszka** i wyszukaj `dragonfly`, a następnie dodaj duszka **ważka**.

![Ikona duszka w interfejsie aplikacji Scratch](images/choose-sprite-icon.png)

![W polu wyszukiwania wpisano „dragonfly”, a w galerii duszek Dragonfly/ważka.](images/dragonfly-search.png)

--- /task ---

--- task ---

Dodaj skrypt, aby duszek **ważka** podążał za wskaźnikiem myszy (lub palcem):

![Ikona duszka Ważka w interfejsie aplikacji Scratch](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] % // to start small
forever
point towards (mouse-pointer v)
move [5] steps
end
```
--- /task ---

--- task ---

**Test:** Kliknij zieloną flagę i spraw, aby duszek **ważka** poruszał się po scenie. Czy ważka porusza się tak, jak można by się spodziewać?

--- /task ---

Kostium ważki nie jest skierowany w prawo, więc głowa duszka **ważka** nie jest skierowana w stronę wskaźnika myszy.

--- task ---

Kliknij zakładkę **Kostiumy** i użyj narzędzia **Wybierz** (strzałka), aby wybrać kostium.

Użyj narzędzia **Obróć** na dole wybranego kostiumu, aby obrócić kostium **ważka** w prawo.

![Animowany obraz pokazujący, jak obrócić kostium ważki, przeciągając strzałki obracania tak, aby ważka była skierowana w prawo.](images/rotated-costume.gif)

--- /task ---

--- task ---

**Test:** Kliknij zieloną flagę i zobacz, jak teraz porusza się ważka.

--- /task ---

Skrzydła ważki wydają dźwięk trzepotania ponieważ wibrują. Możesz edytować dźwięk w Scratch, aby stworzyć własny dźwięk.

--- task ---

Dodaj dźwięk **Crank** do duszka **ważki**.

[[[generic-scratch3-sound-from-library]]]

![](images/crank-sound-editor.png)

--- /task ---

--- task ---

**Test:** Click the **Play** button so you can hear the sound.

--- /task ---

Dźwięk **Crank** jest zbyt długi i zbyt wolny dla skrzydeł ważki.

--- task ---

Wybierz koniec dźwięku za pomocą kursora lub palca.

Kliknij **Skopiuj do nowych**, aby stworzyć nowy dźwięk tylko z wybraną częścią:

![Koniec dźwięku korby wybrany na niebiesko z podświetloną ikoną „Kopiuj do nowego”.](images/crank-copy-end.png)

--- /task ---

--- task ---

Zmień nazwę swojego nowego dźwięku z **Crank2** na `Skrzydła`. ![Właściwość zmiany nazwy dźwięku.](images/crank-wings-sound.png)

--- /task ---

--- task ---

**Test:** Play the new sound. Click the **Faster** button a few times until you like the result:

![A faster sound wave with the 'Faster' icon highlighted.](images/wings-faster.png)

--- /task ---

--- task ---

If you like, you can select the very end of the **Wings** sound, and then click **Delete** to remove it:

![The end of the sound wave selected with the 'Delete' tool highlighted.](images/wings-shorter.png)

--- /task ---

--- task ---

Now add a block to play the **Wings** sound when the dragonfly moves:

![Dragonfly sprite icon](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
```
--- /task ---

--- task ---

**Test:** Try out your dragonfly movement and sound effect.

--- /task ---

--- save ---
