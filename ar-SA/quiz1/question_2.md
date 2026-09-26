
--- question ---
---
legend: Question 2 of 3
---

لقد كتبت شفرة برمجية لجعل اليعسوب يتحرك فقط إذا `لم يكن`{:class="block3operators"} بوضعٍ `ملامس` لمؤشر الماوس.

أين ستضع كتلة `ابدأ الصوت`{:class="block3sound"} لتجعل اليعسوب يصدر صوتًا في كل مرة يتحرك فيها؟

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

لا، باستخدام هذه الشفرة البرمجية، تكون كتلة `ابدأ الصوت`{:class="block3sound"} خارج كتلة `إذا`{:class="block3control"}، لذلك سيتم تشغيلها في كل مرة تعمل بها الكتلة `كرر باستمرار`{:class="block3control"}، حتى لو لم يتحرك اليعسوب.

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

هذا صحيح. وضع كتلة `ابدأ الصوت`{:class="block3sound"} داخل كتلة `اذا`{:class="block3control"} يعني أنه سيتم تشغيله عندما يتحرك اليعسوب.

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

لا، كتلة `ابدأ الصوت`{:class="block3control"} خارج كتلة `إذا`{:class="block3control"}، لذلك سيتم تشغيلها في كل مرة تعمل بها الكتلة `كرر باستمرار`{:class="block3control"}، حتى لو لم يتحرك اليعسوب.

  --- /feedback ---

--- /choices ---

--- /question ---
