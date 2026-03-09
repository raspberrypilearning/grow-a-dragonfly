## Αναστοχασμός

Answer the three questions. There are hints to guide you to the correct answer.

Έχεις χρησιμοποιήσει τα μπλοκ `Συμβάντα`{:class="block3events"}, `Έλεγχος`{:class="block3control"}, `Αισθητήρες`{:class="block3sensing"}, `Τελεστές`{:class="block3operators"}, `Κίνηση`{:class="block3motion"}, `Όψεις`{:class="block3looks"} και `Ήχος`{:class="block3sound"}!

Τώρα ήρθε η ώρα να εξετάσεις τις νέες γνώσεις — ο αναστοχασμός είναι σημαντικό μέρος της μάθησης, επειδή βοηθά στη δημιουργία νέων συνδέσεων στον εγκέφαλό σου.

--- question ---
---
legend: Question 1 of 3
---

A project uses the **Crab** sprite and the **Jellyfish** sprite. The **Crab** sprite has this code:

![desc](images/crab-icon.png)

```blocks3
όταν γίνει κλικ στη σημαία
εάν <not <touching color (#0000FF)?>> τότε
εξαφανίσου
τέλος
```

What would need to happen for the **Crab** sprite to hide?

--- choices ---

- () Το αντικείμενο **Κάβουρας** θα πρέπει να αγγίξει τη **Μέδουσα**

 --- feedback ---

 Όχι, το μπλοκ `εάν`{:class="block3control"} έχει μια συνθήκη `Αισθητήρα`{:class="block3sensing"}, αλλά δεν χρησιμοποιεί το μπλοκ `αγγίζει Μέδουσα`{:class="block3sensing"}.

 --- /feedback ---

- (x) Το αντικείμενο **Κάβουρας** θα πρέπει να μην αγγίζει το μπλε χρώμα

 --- feedback ---

Yes, the `not`{:class="block3operators"} operator means that the condition is true `if`{:class="block3control"} the **Crab** sprite is not `touching`{:class="block3sensing"} the colour blue.

 --- /feedback ---

- () Το αντικείμενο **Κάβουρας** θα πρέπει να αγγίζει το μπλε χρώμα

 --- feedback ---

 Όχι ακριβώς, κοίταξε προσεκτικά τον `τελεστή`{:class="block3operators"} στην συνθήκη.

 --- /feedback ---

- ( ) Το αντικείμενο **Κάβουρας** θα `εξαφανίζεται`{:class="block3looks"} πάντα `όταν γίνει κλικ στη σημαία`{:class="block3events"}

 --- feedback ---

 Όχι, υπάρχει ένα μπλοκ `εάν`{:class="block3control"} στον κώδικα του αντικειμένου **Κάβουρας**, οπότε θα εξαφανίζεται μόνο εάν πληρούται η συνθήκη.

 --- /feedback ---

--- /choices ---

--- /question ---
