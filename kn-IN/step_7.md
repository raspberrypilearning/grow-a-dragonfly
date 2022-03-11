## ಕೀಟದ ಯಾದೃಚ್ಛಿಕ ಚಲನೆ

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ನಿಮ್ಮ ಆಪ್‌ನಲ್ಲಿರುವ ಕೀಟಗಳು ಬಹಳ ಊಹಿಸಬಹುದಾದ ವಿನ್ಯಾಸಗಳಲ್ಲಿ ಚಲಿಸುತ್ತವೆ, ಆದರೆ ನಿಜಜೀವನದಲ್ಲಿ ಅವುಗಳನ್ನು ಹಿಡಿಯುವುದು ಕಷ್ಟ. 

ಕೀಟವು ಹೆಚ್ಚು ಸ್ವಾಭಾವಿಕ ರೀತಿಯಲ್ಲಿ ಚಲಿಸುವಂತೆ ಮಾಡಲು ನೀವು `pick random`{:class="block3operators"} ಬ್ಲಾಕ್‌ ಉಪಯೋಗಿಸುತ್ತೀರಿ.
</div>
<div>
![ಕೀಟಗಳು ಬೇರೆ ಬೇರೆ ದಿಕ್ಕುಗಳನ್ನು ಸೂಚಿಸುತ್ತಿರುವುದನ್ನು ತೋರಿಸುತ್ತಿರುವ Stage.](images/random-movement.png){:width="300px"}
</div>
</div>

--- task ---

ಪ್ರತಿ 1–3 ಸೆಕೆಂಡುಗಳಿಗೆ **Insect 2** ಯಾದೃಚ್ಛಿಕ ದಿಕ್ಕನ್ನು ಸೂಚಿಸುವಂತೆ ಮಾಡಲು ಬರಹವನ್ನು ಸೇರಿಸಿ.

```blocks3
when flag clicked
forever // Keep changing direction
point in direction (pick random [0] to [259])
wait (pick random [1] to [3]) seconds
end
```

--- /task ---

--- task ---

**ಪರೀಕ್ಷೆ:** ನಿಮ್ಮ ಪ್ರಾಜೆಕ್ಟ್‌ನ್ನು ರನ್‌ ಮಾಡಿ ಮತ್ತು ನೋಣ ಹೇಗೆ ಚಲಿಸುತ್ತದೆ ಎಂದು ವೀಕ್ಷಿಸಿ. ನಿಮಗೆ ಬೇಕಾದ ಪರಿಣಾಮ ಪಡೆಯಲು ಸಂಖ್ಯೆಗಳನ್ನು ಬದಲಾಯಿಸಲು ಪ್ರಯತ್ನಿಸಿ.

ನೀವು ಈ ಬರಹವನ್ನು **Insect** ಸ್ಪ್ರೈಟ್‌ಗೂ ಸಹ ಎಳೆದುಹಾಕಬಹುದು, ಅದರಿಂದ ಅದೂ ಸಹ ಯಾದೃಚ್ಛಿಕವಾಗಿ ಚಲಿಸುತ್ತದೆ.

--- /task ---

--- task ---

ಕೀಟಗಳನ್ನು ಅವುಗಳು ನಿಮಗೆ ಬೇಕಾದ ಹಾಗೆ ವರ್ತಿಸುವವರೆಗೆ ಬದಲಾಯಿಸಿ.

ಅವುಗಳನ್ನು ವೇಗ ಅಥವಾ ನೀಧಾನಗೊಳಿಸಲು ನೀವು ಅವುಗಳ `move`{:class="block3motion"} ಹಂತಗಳ ಸಂಖ್ಯೆಯನ್ನು ಬದಲಾಯಿಸಬಹುದು.

ನೀವು ಡ್ರಾಗನ್‌ಫ್ಲೈಯ ವೇಗವನ್ನೂ ಸಹ ಬದಲಾಯಿಸಬಹುದು.

--- /task ---

--- task ---

ಡ್ರಾಗನ್‌ಫ್ಲೈ ಪೂರ್ಣಗಾತ್ರ ತಲುಪಲು ಬೆಳೆಯಬೇಕಾದ ಗಾತ್ರವನ್ನೂ ಸಹ ನೀವು ಬದಲಾಯಿಸಬಹುದು.

ನಿಮ್ಮ ಪ್ರಾಜೆಕ್ಟ್‌ ನಿಮಗೆ ಖುಷಿ ಕೊಡುವವರೆಗೂ ಬದಲಾವಣೆಗಳನ್ನು ಮಾಡಿ.

--- /task ---

--- save ---