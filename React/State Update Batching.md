# Explanation

- Batch Multiple State Updates from [[useState]]
- [[How Components are Displayed on Screen|Render + Commit]] the Batched Single Time
- That's why If console.log(State) After setState you won't find it Updated
    - Because It [[Fiber Tree]] isn't Updated Yet
