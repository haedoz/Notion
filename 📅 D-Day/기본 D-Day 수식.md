## 📝 기본 D-Day 수식


### 기본 style
><img width="485" height="229" alt="스크린샷 2026-07-27 오전 11 43 52" src="https://github.com/user-attachments/assets/1cd04c24-ae84-4b81-96db-478ae3a88b97" />

```javascript
lets(
  d, dateBetween(prop("마감일"), today(), "days"),
  
  if(
  d == 0,
  "D-Day",
  
  if(
    d > 0,
    "D-" + format(d),
    "D+" + format(abs(d))
    )
  )
)
```
<br>
