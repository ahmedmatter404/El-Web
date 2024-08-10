# Explanation

- Special built-in Functions that allow accessing _React Internals_
    - Create and access [[State]] from [[Fiber Tree]]
    - Register side effects and manual dom selection

## Rules

- Hooks called only on _top Level_: not inside blocks
    - to Ensure that hooks called on same order everytime
    - Check Reason in Detail : [[#Why Only on top Level]]
- Hooks called on _React functions_, Not in (regular functions, class components)

### Why Only on top Level

- Hooks are stored in a _Linked List_ in a fiber tree
    - Which means that each hook has a pointer to the next hook
- If the middle hook doesn't get called at any time, the remaining hooks that are referenced by that hook will get lost.
- ![[Pasted image 20240401005721.png]]
-
