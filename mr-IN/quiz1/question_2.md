
--- question ---
---
legend: Question 2 of 3
---

ड्रॅगनफ्लाय माऊस-पॉइंटरला `touching`{:class="block3sensing"} `not`{:class="block3operators"} केवळ तो हलण्यासाठी तुम्ही कोड लिहीलात.

ड्रॅगनफ्लाय प्रत्येक वेळी हलतांना साऊंड करण्यासाठी तुम्ही `start sound`{:class="block3sound"} ब्लॉक कोठे ठेवाल?

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

नाही, या कोडसह `start sound`{:class="block3sound"} ब्लॉक हा `if`{:class="block3control"} ब्लॉकच्या बाहेर आहे, त्यामुळे तो प्रत्येक वेळी `forever`{:class="block3control"} लूप रन होतो, ड्रॅगनफ्लाय हलला नाही तरीसुद्धा.

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

होय, ते बरोबर आहे. `start sound`{:class="block3sound"} ब्लॉक `if`{:class="block3control"} ब्लॉकच्या आत ठेवणे म्हणजे त्यामुळे ड्रॅगनफ्लाय हलतो.

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

नाही, `start sound`{:class="block3sound"} ब्लॉक`if`{:class="block3control"} ब्लॉकच्या बाहेर असल्यास, तो प्रत्येक वेळी `forever`{:class="block3control"} लूप रन होतो, ड्रॅगनफ्लाय हलला नाही तरीसुद्धा.

  --- /feedback ---

--- /choices ---

--- /question ---
