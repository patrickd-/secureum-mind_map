# 56 - [Data Location & Assignments](Data%20Location%20&%20Assignments.md)
Data Location & Assignment: Data locations are not only relevant for persistence of data, but also for the semantics of assignments.

1.  Assignments between storage and memory (or from calldata) always create an independent copy.
    
2.  Assignments from memory to memory only create references. This means that changes to one memory variable are also visible in all other memory variables that refer to the same data.
    
3.  Assignments from storage to a local storage variable also only assign a reference.
    
4.  All other assignments to storage always copy. Examples for this case are assignments to state variables or to members of local variables of storage struct type, even if the local variable itself is just a reference.

___
## Slide Screenshot
![056.png](../images/solidity101/056.png)
___
## Slide Deck
- Data Location -> Persistency & Assignment Semantics
- storage-memory -> copy
- memory-memory -> reference
- storage-storage -> reference
- others -> copy
- Impact: Copy/Modification
- Security: Reference Risk
___
## References
- [Youtube Reference](https://youtu.be/6VIJpze1jbU?t=1835)

___
## Resources
- 