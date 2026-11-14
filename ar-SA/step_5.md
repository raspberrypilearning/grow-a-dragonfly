## تحسين الحركة

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
اليعسوب "فيه خطأ" ويغير اتجاهه بسرعة كبيرة إذا كان مؤشر الماوس يلامس اليعسوب. سوف تتحقق من شرط آخر لإصلاح هذا الخطأ.
</div>
<div>
![تظهر المنصة مع يعسوب وحشرة.](images/improved-movement.png){:width="300px"}
</div>
</div>

--- task ---

اختر كائن **Dragonfly** وابحث عن النص الذي يبدأ بالكتلة `عند نقر العلم`{:class="block3events"}.

اسحب كتلة `إذا`{:class="block3control"} داخل الكتلة `كرر باستمرار`{:class="block3control"} وستتحرك الكتل الموجودة داخل حلقة `كرر باستمرار`{:class="block3control"} في داخل كتلة `إذا`{:class="block3control"}. The blocks inside the `forever`{:class="block3control"} will move inside the `if`{:class="block3control"}.

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+if < > then
start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
end
```
--- /task ---

--- task ---

ثم اسحب كتلة `ليس`{:class="block3operators"} إلى كتلة `إذا`{:class="block3control"} وضع كتلة `ملامس لـ(مؤشر الفأرة)`{:class="block3sensing"} داخلها.

```blocks3
when flag clicked
set size to [25] %
forever
+if <not <touching [mouse-pointer v] ?> > then
start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
end
```

--- /task ---

--- task ---

**اختبار:** تحقق من أن الخلل قد تم إصلاحه، وأن كائن اليعسوب Dragonfly يتحرك فقط عندما `لا`{: class="block3operators"} يكون في حالة `ملامس لـ(مؤشر الفأرة)`{:class="block3sensing"}.

--- /task ---

--- task ---

Try a different condition that makes the dragonfly move when it is far enough from the mouse-pointer:

```blocks3
<(المسافة الى [مؤشر الفأرة v]) > [50]>
```

--- /task ---

--- save ---
