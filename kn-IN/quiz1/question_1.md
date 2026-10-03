## ಪುನರ್ಮನನ

Answer the three questions. There are hints to guide you to the correct answer.

ನೀವು `Events`{:class="block3events"}, `Control`{:class="block3control"}, `Sensing`{:class="block3sensing"}, `Operators`{:class="block3operators"}, `Motion`{:class="block3motion"}, `Looks`{:class="block3looks"}, ಮತ್ತು `Sound`{:class="block3sound"} ಬ್ಲಾಕ್‌ಗಳನ್ನು ಉಪಯೋಗಿಸಿದ್ದೀರಿ!

ಈಗ ಪುನರ್ಮನನ ಮಾಡುವ ಸಮಯ — ಪುನರ್ಮನನ ಕಲಿಕೆಯ ಒಂದು ಮಹತ್ವದ ಭಾಗ, ಏಕೆಂದರೆ ಅದು ನಿಮ್ಮ ಮೆದುಳಿನಲ್ಲಿ ಹೊಸ ಸಂಪರ್ಕಗಳನ್ನು ಮಾಡಲು ಸಹಾಯ ಮಾಡುತ್ತದೆ.

--- question ---
---
legend: Question 1 of 3
---

A project uses the **Crab** sprite and the **Jellyfish** sprite. The **Crab** sprite has this code:

![desc](images/crab-icon.png)

```blocks3
when flag clicked
if <not <touching color (#0000FF)?>> then
hide
end
```

What would need to happen for the **Crab** sprite to hide?

--- choices ---

- () **Crab** ಸ್ಪ್ರೈಟ್ **Jellyfish**ನ್ನು ಸ್ಪರ್ಶಿಸಬೇಕು

 --- feedback ---

 ಇಲ್ಲ, `if`{:class="block3control"} ಬ್ಲಾಕ್‌ `Sensing`{:class="block3sensing"} ಷರತ್ತು ಹೊಂದಿದೆ, ಆದರೆ ಅದು `touching Jellyfish`{:class="block3sensing"} ಬ್ಲಾಕ್‌ ಉಪಯೋಗಿಸುವುದಿಲ್ಲ.

 --- /feedback ---

- (x) **Crab** ಸ್ಪ್ರೈಟ್‌ ನೀಲಿ ಬಣ್ಣವನ್ನು ಸ್ಪರ್ಶಿಸುತ್ತಿರಬಾರದು

 --- feedback ---

Yes, the `not`{:class="block3operators"} operator means that the condition is true `if`{:class="block3control"} the **Crab** sprite is not `touching`{:class="block3sensing"} the colour blue.

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
