
--- question ---
---
legend: Ερώτηση 2 από 3
---

Έγραψες κώδικα για να κάνεις τη λιβελούλα να κινείται μόνο αν είναι `δεν`{:class="block3operators"} `αγγίζει`{:class="block3sensing"} τον δείκτη του ποντικιού.

Πού θα έβαζες ένα μπλοκ `παίξε ήχο`{:class="block3sound"} για να κάνεις τη λιβελούλα να ξεκινά έναν ήχο κάθε φορά που κινείται;

--- choices ---

- ( )

```blocks3
when flag clicked
forever
+start sound [Φτερά v]
if <not <touching [mouse-pointer v] ?> > then
point towards (mouse-pointer v)
move [5] steps
end
end
```

--- feedback ---

Όχι, με αυτόν τον κώδικα το μπλοκ `παίξε ήχο`{:class="block3sound"} βρίσκεται εκτός του μπλοκ `εάν`{:class="block3control"}, επομένως θα εκτελείται κάθε φορά που ο βρόγχος `για πάντα`{:class="block3control"} εκτελείται, ακόμα κι αν η λιβελούλα δεν κινείται.

--- /feedback ---

- (x)

```blocks3
when flag clicked
forever
if <not <touching [mouse-pointer v] ?> > then
+start sound [Φτερά v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

  --- feedback ---

Ναι, αυτό είναι σωστό. Τοποθετώντας το μπλοκ `παίξε ήχο`{:class="block3sound"} μέσα στο μπλοκ `εάν`{:class="block3control"} σημαίνει ότι θα παίζει όταν κινείται η λιβελούλα.

  --- /feedback ---

- ( )


```blocks3
when flag clicked
forever
if <not <touching [mouse-pointer v] ?> > then
point towards (mouse-pointer v)
move [5] steps
end
+start sound [Φτερά v]
end
```

  --- feedback ---

Όχι, με αυτόν τον κώδικα το μπλοκ `παίξε ήχο`{:class="block3sound"} βρίσκεται εκτός του μπλοκ `εάν`{:class="block3control"}, επομένως θα εκτελείται κάθε φορά που ο βρόγχος `για πάντα`{:class="block3control"} εκτελείται, ακόμα κι αν η λιβελούλα δεν κινείται.

  --- /feedback ---

--- /choices ---

--- /question ---
