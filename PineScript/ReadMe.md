### Scope every indicator
```js
//@version=4
study("Green Bars Count")
var count = 0
isGreen = close >= open
if isGreen
    count := count + 1
plot(count)
```
