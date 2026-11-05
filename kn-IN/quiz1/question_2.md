
--- question ---
---
legend: Question 2 of 3
---

ಡ್ರಾಗನ್‌ಫ್ಲೈ `not`{:class="block3operators"} `touching`{:class="block3sensing"} ಮೌಸ್-ಪಾಯಿಂಟರ್‌ ಆಗಿದ್ದರೆ ಮಾತ್ರ ಅದು ಚಲಿಸುವಂತೆ ಮಾಡಲು ನೀವು ಕೋಡ್‌ ಬರೆದಿರಿ.

ಡ್ರಾಗನ್‌ಫ್ಲೈ ಪ್ರತಿ ಬಾರಿ ಚಲಿಸಿದಾಗ ಅದು ಶಬ್ದ ಮಾಡಲು ಪ್ರಾರಂಭಿಸಲು ನೀವು `start sound`{:class="block3sound"} ಬ್ಲಾಕ್‌ ಎಲ್ಲಿ ಇರಿಸುವಿರಿ?

--- choices ---

- ( )

```blocks3
when flag clicked
forever
+start sound [Wings v]
if <not <touching [mouse-pointer v] ?> > then
point towards (mouse-pointer v)
move [5] steps
end
end
```

--- feedback ---

ಇಲ್ಲ, ಈ ಕೋಡ್‌ನಿಂದ `start sound`{:class="block3sound"} ಬ್ಲಾಕ್ `if`{:class="block3control"} ಬ್ಲಾಕ್‌ ಹೊರಗಡೆ ಇದೆ, ಆದುದರಿಂದ, ಡ್ರಾಗನ್‌ಫ್ಲೈ ಚಲಿಸದಿದ್ದರೂ, `forever`{:class="block3control"} ಲೂಪ್‌ ರನ್‌ ಆದಾಗ, ಇದು ಪ್ರತಿಬಾರಿ ರನ್‌ ಆಗುತ್ತದೆ.

--- /feedback ---

- (x)

```blocks3
when flag clicked
forever
if <not <touching [mouse-pointer v] ?> > then
+start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

  --- feedback ---

ಹೌದು, ಅದು ಸರಿಯಾಗಿದೆ. `start sound`{:class="block3sound"} ಬ್ಲಾಕ್‌ನ್ನು `if`{:class="block3control"} ಬ್ಲಾಕ್‌ ಒಳಗೆ ಇಡುವುದು ಎಂದರೆ ಅದು ಡ್ರಾಗನ್‌ಫ್ಲೈ ಚಲಿಸಿದಾಗ ನುಡಿಸುತ್ತದೆ.

  --- /feedback ---

- ( )


```blocks3
when flag clicked
forever
if <not <touching [mouse-pointer v] ?> > then
point towards (mouse-pointer v)
move [5] steps
end
+start sound [Wings v]
end
```

  --- feedback ---

ಇಲ್ಲ, `start sound`{:class="block3sound"} ಬ್ಲಾಕ್ `if`{:class="block3control"} ಬ್ಲಾಕ್‌ ಹೊರಗಡೆ ಇದೆ, ಆದುದರಿಂದ, ಡ್ರಾಗನ್‌ಫ್ಲೈ ಚಲಿಸದಿದ್ದರೂ, ಅದು `forever`{:class="block3control"} ಲೂಪ್‌ ರನ್‌ ಆದಾಗ ಪ್ರತಿಬಾರಿ ರನ್‌ ಆಗುತ್ತದೆ.

  --- /feedback ---

--- /choices ---

--- /question ---
