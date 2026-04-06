---
layout: default
title: "Unit 2 Task 26 - Solution"
permalink: /tasks/2-26-solution/
---

# Solution - Task 26: BMI and health band

[← Back to task]({{ site.baseurl }}/tasks/2-26/)

---

One possible program:

```python
while True:
    h = float(input("Height (m): "))
    w = float(input("Weight (kg): "))
    if h > 0 and w > 0:
        break
    print("Height and weight must be positive.")

bmi = w / (h * h)
print("BMI:", round(bmi, 2))

if bmi < 18.5:
    print("underweight")
elif bmi < 25:
    print("normal")
elif bmi < 30:
    print("overweight")
else:
    print("obese")
```
