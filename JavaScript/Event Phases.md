# Explanation

## Phases

![[Capturing, Bubbling.png]]

1. _Capturing Phase_: event Travels from root Dom to target element
    - Make use of it by using [[Event Delegation]]
2. _Target Phase_: apply callback
3. _Bubling Phase_: event travels to parent element back
    - events are executed in this phase by default
    - [[Event Propagation]]

## Note

- callback functions are applied to each parent element has the event
- Stopped by `e.stopPropogation()`

# Sources
