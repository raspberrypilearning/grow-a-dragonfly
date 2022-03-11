## جهز المشهد

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
سوف تقوم بإعداد المشهد. اختر الخلفية الخاصة بك وأضف اليعسوب الذي يتبع مؤشر الماوس حول المنصة.
</div>
<div>
![](images/set-the-scene.png){:width="300px"}
</div>
</div>

--- task ---

افتح [مشروع البداية كبّر اليعسوب](https://scratch.mit.edu/projects/535695413/editor){:target="_blank"}. سيتم فتح Scratch في علامة تبويب متصفح أخرى.

[[[working-offline]]]

--- /task ---

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">** اليعاسيب **</span> يمكن العثور عليها في جميع أنحاء العالم وهي موجودة منذ أكثر من 300 مليون سنة!</p>

--- task ---

**اختر:** انقر فوق **اختيار خلفية** وأضف خلفية من اختيارك. استخدمنا خلفية **Jurassic**.

![](images/choose-backdrop-icon.png)

![تُظهر المنصةُ الخلفيةَ Jurassic.](images/Jurassic-backdrop.png)

--- /task ---

--- task ---

انقر فوق **اختيار كائن** وابحث عن كلمة `dragonfly`، ثم أضف كائن **Dragonfly**.

![](images/choose-sprite-icon.png)

![مربع البحث المكتوب فيه "dragonfly" وكائن اليعسوب في المعرض.](images/dragonfly-search.png)

--- /task ---

--- task ---

أضف نصًّا لجعل الكائن **Dragonfly** يتبع مؤشر الماوس (أو إصبعك):

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] % // to start small
forever
point towards (mouse-pointer v)
move [5] steps
end
```
--- /task ---

--- task ---

**اختبار:** انقر فوق العلم الأخضر واجعل الكائن **Dragonfly** يتحرك حول المنصة. هل اليعسوب يتحرك كما تتوقع؟

--- /task ---

لا يتجه مظهر اليعسوب إلى اليمين، لذا فإن رأس الكائن **Dragonfly** لا يشير إلى مؤشر الماوس.

--- task ---

انقر فوق علامة التبويب **المظاهر** واستخدم أداة **حدد** (السهم) لتحديد الزي. استخدم أداة **دوّر** في الجزء السفلي من الزي المحدد لقلب شكل الكائن **Dragonfly** لمواجهة اليمين.

![صورة متحركة توضح كيفية تدوير زي اليعسوب عن طريق سحب أسهم الدوران بحيث تواجه اليعسوب جهة اليمين.](images/rotated-costume.gif)

![تم اختيار زي اليعسوب واستدار لمواجهة اليمين.](images/rotated-costume.png)

--- /task ---

--- task ---

**اختبار:** انقر على العلم الأخضر وشاهد كيف يتحرك اليعسوب.

--- /task ---

تُصدر أجنحة اليعسوب صوت رفرفة أثناء اهتزازها. يمكنك تحرير الصوت في Scratch لإنشاء الصوت الخاص بك.

--- task ---

أضف صوت **Crank** إلى كائن **Dragonfly**.

[[[generic-scratch3-sound-from-library]]]

![](images/crank-sound-editor.png)

انقر فوق الزر **تشغيل** حتى تتمكن من سماع الصوت.

--- /task ---

صوت ** Crank ** طويل جدًّا وبطيء جدًّا بالنسبة لأجنحة اليعسوب.

--- task ---

حدد نهاية الصوت باستخدام المؤشر أو الإصبع.

انقر فوق **نسخ إلى صوت جديد** لإنشاء صوت جديد بالجزء المحدد فقط:

![تحديد نهاية صوت crank باللون الأزرق مع تمييز رمز "نسخ إلى صوت جديد".](images/crank-copy-end.png)

أعد تسمية صوتك الجديد من **Crank2** إلى `أجنحة`.

![خاصية إعادة تسمية الصوت.](images/crank-wings-sound.png)

--- /task ---

--- task ---

قم بتشغيل الصوت الجديد. انقر فوق الزر **تسريع** عدة مرات إلى أن تعجبك النتيجة:

![موجة صوتية أسرع مع تمييز الرمز "تسريع".](images/wings-faster.png)

--- /task ---

--- task ---

إذا أردت، يمكنك تحديد نهاية الصوت **أجنحة**، ثم النقر فوق **حذف** لإزالته:

![نهاية الموجة الصوتية مُحدَّدة، مع أداة "حذف" المؤشَّرة.](images/wings-shorter.png)

--- /task ---

--- task ---

أضف الآن كتلة لتشغيل صوت **أجنحة** عندما يتحرك اليعسوب:

![](images/dragonfly-icon.png)

```blocks3
when flag clicked
set size to [25] %
forever
+start sound [Wings v]
point towards (mouse-pointer v)
move [5] steps
end
```
--- /task ---

--- task ---

**اختبار:** جرب حركة اليعسوب وتأثير الصوت.

--- /task ---

--- save ---
