## ಪುನರ್ಮನನ

ಭೇಷ್, ಬಳಕೆದಾರ ನಿಯಂತ್ರಿಸುವ ಡ್ರಾಗನ್‌ಫ್ಲೈ ಮತ್ತು ಒಂದು ಕ್ರಮಾವಳಿಯನ್ನು ಅನುಸರಿಸುವ ಕೀಟಗಳೊಂದಿಗೆ ನೀವು ಪ್ರಕೃತಿ ಆಪ್‌ ರಚಿಸಿದ್ದೀರಿ!

ನೀವು `Events`{:class="block3events"}, `Control`{:class="block3control"}, `Sensing`{:class="block3sensing"}, `Operators`{:class="block3operators"}, `Motion`{:class="block3motion"}, `Looks`{:class="block3looks"}, ಮತ್ತು `Sound`{:class="block3sound"} ಬ್ಲಾಕ್‌ಗಳನ್ನು ಉಪಯೋಗಿಸಿದ್ದೀರಿ!

ಈಗ ಪುನರ್ಮನನ ಮಾಡುವ ಸಮಯ — ಪುನರ್ಮನನ ಕಲಿಕೆಯ ಒಂದು ಮಹತ್ವದ ಭಾಗ, ಏಕೆಂದರೆ ಅದು ನಿಮ್ಮ ಮೆದುಳಿನಲ್ಲಿ ಹೊಸ ಸಂಪರ್ಕಗಳನ್ನು ಮಾಡಲು ಸಹಾಯ ಮಾಡುತ್ತದೆ.

ನೀವು ಕಲಿತಿದ್ದನ್ನು ಪುನರ್ಮನನ ಮಾಡಲು ಈ ಕೆಳಗಿನ ಮೂರು ಪ್ರಶ್ನೆಗಳಿಗೆ ಉತ್ತರಿಸಿ.

ಪ್ರತಿಯೊಂದು ಪ್ರಶ್ನೆಯ ನಂತರ, ಸಬ್ಮಿಟ್‌ ಒತ್ತಿ. ಸರಿಯಾದ ಉತ್ತರದೆಡೆಗೆ ನಿಮಗೆ ಮಾರ್ಗದರ್ಶನ ನೀಡಲಾಗುತ್ತದೆ. ಈ ಚಟುವಟಿಕೆಯನ್ನು ನೀವು ಎಷ್ಟು ಸಲ ಬೇಕಾದರೂ ಮಾಡಬಹುದು.

ಆನಂದಿಸಿ!

--- question ---
---
legend: 3 ಪ್ರಶ್ನೆಗಳಲ್ಲಿ 1ನೆಯದು
---

ಪ್ರಾಜೆಕ್ಟೊಂದು **Crab** ಸ್ಪ್ರೈಟ್‌ ಮತ್ತು **Jellyfish** ಸ್ಪ್ರೈಟ್‌ ಉಪಯೋಗಿಸುತ್ತದೆ. **Crab** ಸ್ಪ್ರೈಟ್‌ ಈ ಕೋಡ್‌ ಹೊಂದಿದೆ:

![desc](images/crab-icon.png)

```blocks3
when flag clicked
if <not <touching color (#0000FF)?>> then
hide
end
```

**Crab** ಸ್ಪ್ರೈಟ್‌ ಮರೆಮಾಡಲು ಏನಾಗಬೇಕು?

--- choices ---

- () **Crab** ಸ್ಪ್ರೈಟ್ **Jellyfish**ನ್ನು ಸ್ಪರ್ಶಿಸಬೇಕು

 --- feedback ---

 ಇಲ್ಲ, `if`{:class="block3control"} ಬ್ಲಾಕ್‌ `Sensing`{:class="block3sensing"} ಷರತ್ತು ಹೊಂದಿದೆ, ಆದರೆ ಅದು `touching Jellyfish`{:class="block3sensing"} ಬ್ಲಾಕ್‌ ಉಪಯೋಗಿಸುವುದಿಲ್ಲ.

 --- /feedback ---

- (x) **Crab** ಸ್ಪ್ರೈಟ್‌ ನೀಲಿ ಬಣ್ಣವನ್ನು ಸ್ಪರ್ಶಿಸುತ್ತಿರಬಾರದು

 --- feedback ---

ಹೌದು, `not`{:class="block3operators"} ಆಪರೇಟರ್‌ ಎಂದರೆ `if`{:class="block3control"} **Crab** ಸ್ಪ್ರೈಟ್ ನೀಲಿ ಬಣ್ಣ `touching`{:class="block3sensing"} ಸ್ಪರ್ಶಿಸುತ್ತಿಲ್ಲ ಎನ್ನುವ ಷರತ್ತು ಸರಿಯಾಗಿರುತ್ತದೆ.

 --- /feedback ---

- () **Crab** ಸ್ಪ್ರೈಟ್‌ ನೀಲಿ ಬಣ್ಣವನ್ನು ಸ್ಪರ್ಶಿಸುತ್ತಿರಬೇಕು

 --- feedback ---

 ಅಷ್ಟು ಸರಿಯಾಗಿಲ್ಲ, ಷರತ್ತಿನಲ್ಲಿ `operator`{:class="block3operators"} ಕಡೆಗೆ ಸೂಕ್ಷ್ಮವಾಗಿ ಗಮನಿಸಿ.

 --- /feedback ---

- ( ) **Crab** ಸ್ಪ್ರೈಟ್‌ ಯಾವಾಗಲೂ `hide`{:class="block3looks"} `when the flag is clicked`{:class="block3events"}

 --- feedback ---

 ಇಲ್ಲ, **Crab** ಸ್ಪ್ರೈಟ್‌ ಕೋಡ್‌ನಲ್ಲಿ `if`{:class="block3control"} ಬ್ಲಾಕ್‌ ಇದೆ, ಆದುದರಿಂದ ಷರತ್ತು ಪೂರೈಕೆಯಾದರೆ ಮಾತ್ರ ಅದು ಮರೆಯಾಗುತ್ತದೆ.

 --- /feedback ---

--- /choices ---

--- /question ---
