## Quick quiz

Answer the three questions. There are hints to guide you to the correct answer.

When you have answered each question, click on **Check my answer**.

Have fun!

--- question ---
---
legend: السؤال 1 من 3
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

- () سيحتاج الكائن **Crab** إلى لمس كائن **Jellyfish**

 --- feedback ---

 لا، كتلة `إذا`{:class="block3control"} تحتوي على شرط `تحسس`{:class="block3sensing"}، لكنها لا تستخدم كتلة Jellyfish `ملامس لـ`{:class="block3sensing"}.

 --- /feedback ---

- (x) يجب ألا يلامس الكائن **Crab** اللون الأزرق

 --- feedback ---

Yes, the `not`{:class="block3operators"} operator means that the condition is true `if`{:class="block3control"} the **Crab** sprite is not `touching`{:class="block3sensing"} the colour blue.

 --- /feedback ---

- () يجب أن يلامس الكائن **Crab** اللون الأزرق

 --- feedback ---

 ليس تمامًا، انظر عن كثب إلى `العملية`:class="block3operators"} المستخدمة في الشرط.

 --- /feedback ---

- () سوف `يختفي`{:class="block3looks"} الكائن **Crab** دائمًا `عند نقر العلم`{:class="block3events"}

 --- feedback ---

 لا، هناك كتلة `إذا`{:class="block3control"} في الشفرة البرمجية لكائن**Crab** لذلك ستختفي فقط إذا تحقق الشرط.

 --- /feedback ---

--- /choices ---

--- /question ---
