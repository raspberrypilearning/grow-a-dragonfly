
--- question ---
---
legend: Question 2 of 3
---

आपने ड्रैगनफ्लाई को केवल तभी स्थानांतरित करने के लिए कोड लिखा था जब वह माउस-पॉइंटर को `not`{:class="block3operators"} `touch`{:class="block3sensing"} हो।

ड्रैगनफ्लाई के हर बार हिलने पर ध्वनि शुरू करने के लिए आप `start sound`{:class="block3sound"} ब्लॉक कहां रखेंगे?

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

नहीं, इस कोड के साथ `start sound`{:class="block3sound"} ब्लॉक `if`{:class="block3control"} ब्लॉक के बाहर है, इसलिए यह हर बार जब `forever`{:class="block3control"} लूप चलता है यह भी चलेगा, भले ही ड्रैगनफ्लाई न हिले।

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

हाँ, यह सही है। `start sound`{:class="block3sound"} ब्लॉक को `if`{:class="block3control"} के अंदर ब्लॉक करने का मतलब है कि यह ड्रैगनफ्लाई के चलने पर बजने लगेगा।

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

नहीं, `start sound`{:class="block3sound"} ब्लॉक `if`{:class="block3control"} ब्लॉक के बाहर है, इसलिए यह हर बार `हमेशा के लिए`{:class="block3control"} लूप चलता है यह भी चलेगा, भले ही ड्रैगनफ्लाई न हिले।

  --- /feedback ---

--- /choices ---

--- /question ---
