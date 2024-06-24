# Explanation

![[Pasted image 20240618154959.png]]

- if add an event to inner or nested component
- this event will trigger all callback of parent components
- the solution to this is

```js
e.stopPropagation()
```
