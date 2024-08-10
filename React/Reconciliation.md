# Explanation

- When Componenets are re-rendered, You need to keep elements that doesn't change as they are
- So _Reconcilation Proccess_ Wants to Use as much current Dom as possible
- The dom won't be all updated, the only changed ones
- _Reconciler_
    - Decides which dom element to be updated
    - Called Fiber
- So We Reconcile Current [[Virtual Dom]] with [[Fiber Tree]]
- Illustration: ![[Fiber Tree.png]]
