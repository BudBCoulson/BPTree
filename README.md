# BPTree
Haskell implementations of a B+ Tree.

A B+ Tree is a type of finitely branching tree storing keys and values. See [Wikipedia]() for more details. It is suitable for being used as the backend of a database system.

These two implementations use the same basic ideas but have some differences:
* Version 1 uses a sort of state machine to store parent and child pointers, which allows for easily moving directly to any given node at any time.
* Version 2 has a more clever use of recursion which allows for handling the pointers in the functions directly, but doesn't maintain linkages of the leaves directly.
