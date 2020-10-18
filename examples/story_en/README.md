# dialog unit: puppy



```
       start
           |   .-------------------------------.
   unit1   |   |                               |
  .--------|---|-------------------------.     |
  |        |   |                         |     |
  |        v   v       .-------------.   |     |
  | dogIntroduction -> |presentations|   |     |
  |                    .-------------.   |     |
  |                      |          ^    |     |
  |                      v          |    |     |
  |               +--- pattern 1    |    |     |
  |               |    pattern 2 ->-+    |     |
  |               |    pattern 3 ->-+    |     |
  |               |    default   ->-+    |     |
  |               |                 |    |     |
  |               |    .----------. |    |     |
  |               +--> |verifyName| |    |     |
  |                    .----------. |    |     |
  |                      |          ^    |     |
  |                      v          |    |     |
  |      .------------ pattern 1    |    |     |    
  |      |             pattern 2 ->-+    |     |
  |      |             default   ->-+    |     |
  |      |                               |     |
  |      |                               |     |
  .------|-------------------------------.     |
         |                                     |
         |                                     |
         |                                     |
   unit2 |                                     |
  .------|-------------------------------.     |
  |      |                               |     |
  |      v        .-------.              |     |
  | askRestart -> |restart|              |     |
  |               .-------.              |     |
  |                ^     |               |     |
  |                |     v               |     |
  |                |    pattern 1 -->----------.
  |                |    pattern 2 --.    |
  |                +-<- default     |    |
  |                                 |    |
  .---------------------------------|----.
                                    |
                                    v
                                    exit
```
