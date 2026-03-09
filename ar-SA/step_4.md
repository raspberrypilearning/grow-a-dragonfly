## تنمو إلى الحجم الكامل

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ستجعل اليعسوب ينمو كلما أكل ذبابة، ويتوقف عن النمو إذا وصل إلى الحجم الكامل.
</div>
<div>
![اليعسوب بالحجم الكامل على المنصة وهو يقول "لقد اكتمل نموي!".](images/grow-to-fullsize.png){:width="300px"}
</div>
</div>

The Dragonfly needs to grow when it eats a fly.

عندما تريد السماح لكائن آخر بمعرفة حدوث شيء ما، يمكنك استخدام كتلة `بث`{:class="block3events"} كما فعلت في [بث التعويذات](https://projects.raspberrypi.org/en/projects/broadcasting-spells){:target="_blank"}.

--- task ---

أضف كتلة `بث`{:class="block3events"} إلى كائن الحشرة **Insect** مع الرسالة الجديدة `طعام`{:class="block3events"}:

![](images/fly-icon.png)

```blocks3
when flag clicked
show // show at the start
forever
move [3] steps
if on edge, bounce
if <touching [Dragonfly v] ?> then
+broadcast [food v]
hide
go to (random position v)
wait [1] seconds
show
end
end
```
--- /task ---

يحتاج كائن اليعسوب **Dragonfly** إلى النمو عندما يتلقى الرسالة `طعام`{:class="block3events"}.

--- task ---

حدد الكائن **Dragonfly** وأضف هذا النص:

![](images/dragonfly-icon.png)

```blocks3 
when I receive [food v]
change size by [5]
```

--- /task ---

--- task ---

أضف صوت **Chomp** إلى اليعسوب و`ابدأ الصوت`{:class="block3sound"} عندما تؤكل الحشرة:

```blocks3 
when I receive [food v]
+start sound [Chomp v]
change size by [5]
```
--- /task ---

--- task ---

**اختبار:** قم بتشغيل مشروعك لاختبار نمو اليعسوب وإصدار صوت القضم عندما يأكل ذبابة.

--- /task ---

عندما يصل اليعسوب إلى حجمه الكامل، ستهنئك اللعبة وتتوقف.

--- task ---

أضف كتلة `إذا`{:class="block3control"}.

```blocks3
when I receive [طعام v]
start sound [Chomp v]
change size by [5]
+if <[ ] = [ ]> then
end
```

--- /task ---

يصبح اليعسوب بالحجم الكامل عندما يكون `الحجم`{:class="block3looks"} `=`{:class="block3operators"} `100%`.

--- task ---

أولًا، أضف العملية `=`{:class="block3operators"} إلى الإدخال على الشكل السداسي:

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
+if <[ ] = [ ]> then
end
```
--- /task ---

--- task ---

قم بإنهاء بناء الشرط بإضافة متغير `الحجم`{:class="block3looks"} واكتب القيمة `100`:

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
+if <(size) = [100]> then
end
```
--- /task ---

--- task ---

أضف الكتل بحيث يكون الشرط داخل كتلة `إذا`{:class="block3control"} صحيحًا، `ثم`{:class="block3control"} يقوم اليعسوب بـ `بث`{:class="block3events"} رسالة "النهاية" و`يقول`{:class="block3looks"} `اكتمل نموي!`

وأخيرًا، قم باضافة كتلة `إيقاف الكل`{:class="block3control"} لإيقاف باقي النصوص البرمجية لليعسوب:

```blocks3
when I receive [food v]
start sound [Chomp v]
change size by [5]
if <(size) = [100]> then
+broadcast [end v]
+say [I got to full size!]
+stop [other scripts in sprite v] // change from 'all'
end
```
--- /task ---

--- task ---

في الوقت الحالي، لا زالت الذبابة تتحرك حتى بعد انتهاء تنفيذ المشروع. أضف هذا البرنامج النصي إلى كائن الحشرة ** Insect **.

![](images/fly-icon.png)

```blocks3
when I receive [end v]
stop [other scripts in sprite v]
```

--- /task ---

--- task ---

**اختبار:** انقر فوق العلم الأخضر واستمر في أكل الذباب حتى يصل اليعسوب إلى حجمه الكامل.

--- /task ---

--- save ---
