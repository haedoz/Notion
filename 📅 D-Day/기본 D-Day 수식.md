## 📝 기본 D-Day 수식


### 기본 style
><img width="494" height="184" alt="스크린샷 2026-07-27 오후 12 12 04" src="https://github.com/user-attachments/assets/db0301ec-a646-47c7-99e2-c972b2fe1448" />

```javascript
lets(
  d,
  dateBetween(prop("마감일"), today(), "days"),

  ifs(
    d > 0,
    "D-" + format(d),

    d == 0,
    "D-DAY",

    d < 0,
    ("D+" + format(abs(d))).style("gray")
  )
)
```
<br>
