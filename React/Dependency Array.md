# Explanation

- hook gets Executed [[Asynchronously]] on dependency array change
- Used Also to Synchronize _state_ with _side effects or API_ ![[Pasted image 20240304133716.png]]
- determine when to execute effectHook:![[Pasted image 20240304132925.png]]
- mount
- commit
- browser paint
- effect
    - If doesn't Change state: do nothing
    - otherwise re-render

## Rules

1. add all [[props]], state variables, and contexts to dependency array
2. add all reactive values must be included
    1. _Reactive Values_: values that reference probs, states, and contexts
3. don't Include objects or arrays 1. Because objects with same values are different `{}!=={}`
   ![[Rules to Remove unnecessary dependencies.png]]
