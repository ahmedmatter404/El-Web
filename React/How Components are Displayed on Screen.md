# Explanation

> [!error]- Rendering
>
> -   Happens Internally and has no relation
> -   Has No Relation with Displaying dom on Screen

- Illustration of All Steps: ![[From Trigger to UI Recap.png]]

1. Trigger a Render
    1. Initial Render
    2. Re-render: By Updating State in any _component instance_
2. Rendering Phase: Follows some [[React  Logic]]
    1. Calls Component Functions: which Creates _React Elements_ returned from component Instance
    2. _React Elements_ makes up a new [[Virtual Dom]]
    3. this virtual dom is [[Reconciliation|Reconciled]] + [[Diffing|Diffed]] with current [[Fiber Tree]] to create a an Updated one
3. Commit Phase
    1. Commit is Synchronous: To not show partial results
    2. Take the List of Dom Updates and Commit them Using _ReactDom_
    3. The one responsible for Commit is different hosts
        - React Dom
        - React Native
        - Remotion
        - and Others ...
4. Browser Paint
5. Execute Effect [[useEffect]]
    - If it changes State, re-render
    - Otherwise just execute without re-render
    - Illustration ![[Pasted image 20240304134409.png]]
