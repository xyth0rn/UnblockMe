# UnblockMe

## Usage
work with python2

## Unblock Me FREE Game
https://play.google.com/store/apps/details?id=com.kiragames.unblockmefree


### [1] edit the numberList in the unblockMe.py

```
numberList = [   0,-2, 2, 0,-2, 0, \
                 0, 0, 2, 0, 0, 0, \
                 1, 0,-2,-3, 0, 0, \
                -3, 0, 0, 0, 0, 0, \
                 0, 0,-2, 0, 2, 0, \
                 0, 0, 0, 3, 0, 0]

Note: only need to label the index of each brick in the upper left block
index
 0 = space
 1 = vertical target brick of length 2 
 2 = horizontal brick of length 2
-2 = vertical   brick of length 2
 3 = horizontal brick of length 2
-3 = vertical   brick of length 3
```


### [2] python unblockMe.py
```
========================================
Need 47 moves to solve this puzzle: ((4, 'down'), (10, 'down'), (8, 'right'), (14, 'up'), (26, 'up'), (2, 'right'), (8, 'up'), (12, 'right'), (33, 'left'), (18, 'up'), (32, 'left'), (31, 'left'), (15, 'down'), (13, 'right'), (1, 'down'), (7, 'down'), (13, 'down'), (14, 'left'), (21, 'up'), (30, 'right'), (31, 'right'), (32, 'right'), (20, 'down'), (12, 'down'), (13, 'left'), (2, 'down'), (8, 'down'), (9, 'left'), (8, 'left'), (7, 'left'), (3, 'left'), (2, 'left'), (1, 'left'), (14, 'up'), (8, 'up'), (12, 'right'), (18, 'up'), (26, 'up'), (33, 'left'), (32, 'left'), (31, 'left'), (15, 'down'), (16, 'up'), (10, 'up'), (13, 'right'), (14, 'right'), (15, 'right'))
========================================
---------------
|   4 2 2 4   |
|   4 2 2 4   |
| 1 1 4 5    
| 5   4 5     |
| 5   4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#1: (4, 'down')
---------------
|   4 2 2     |
|   4 2 2 4   |
| 1 1 4 5 4  
| 5   4 5     |
| 5   4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#2: (10, 'down')
---------------
|   4 2 2     |
|   4 2 2     |
| 1 1 4 5 4  
| 5   4 5 4   |
| 5   4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#3: (8, 'right')
---------------
|   4 2 2     |
|   4   2 2   |
| 1 1 4 5 4  
| 5   4 5 4   |
| 5   4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#4: (14, 'up')
---------------
|   4 2 2     |
|   4 4 2 2   |
| 1 1 4 5 4  
| 5     5 4   |
| 5   4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#5: (26, 'up')
---------------
|   4 2 2     |
|   4 4 2 2   |
| 1 1 4 5 4  
| 5   4 5 4   |
| 5   4 5 2 2 |
| 5     3 3 3 |
---------------
move#6: (2, 'right')
---------------
|   4   2 2   |
|   4 4 2 2   |
| 1 1 4 5 4  
| 5   4 5 4   |
| 5   4 5 2 2 |
| 5     3 3 3 |
---------------
move#7: (8, 'up')
---------------
|   4 4 2 2   |
|   4 4 2 2   |
| 1 1   5 4  
| 5   4 5 4   |
| 5   4 5 2 2 |
| 5     3 3 3 |
---------------
move#8: (12, 'right')
---------------
|   4 4 2 2   |
|   4 4 2 2   |
|   1 1 5 4  
| 5   4 5 4   |
| 5   4 5 2 2 |
| 5     3 3 3 |
---------------
move#9: (33, 'left')
---------------
|   4 4 2 2   |
|   4 4 2 2   |
|   1 1 5 4  
| 5   4 5 4   |
| 5   4 5 2 2 |
| 5   3 3 3   |
---------------
move#10: (18, 'up')
---------------
|   4 4 2 2   |
|   4 4 2 2   |
| 5 1 1 5 4  
| 5   4 5 4   |
| 5   4 5 2 2 |
|     3 3 3   |
---------------
move#11: (32, 'left')
---------------
|   4 4 2 2   |
|   4 4 2 2   |
| 5 1 1 5 4  
| 5   4 5 4   |
| 5   4 5 2 2 |
|   3 3 3     |
---------------
move#12: (31, 'left')
---------------
|   4 4 2 2   |
|   4 4 2 2   |
| 5 1 1 5 4  
| 5   4 5 4   |
| 5   4 5 2 2 |
| 3 3 3       |
---------------
move#13: (15, 'down')
---------------
|   4 4 2 2   |
|   4 4 2 2   |
| 5 1 1   4  
| 5   4 5 4   |
| 5   4 5 2 2 |
| 3 3 3 5     |
---------------
move#14: (13, 'right')
---------------
|   4 4 2 2   |
|   4 4 2 2   |
| 5   1 1 4  
| 5   4 5 4   |
| 5   4 5 2 2 |
| 3 3 3 5     |
---------------
move#15: (1, 'down')
---------------
|     4 2 2   |
|   4 4 2 2   |
| 5 4 1 1 4  
| 5   4 5 4   |
| 5   4 5 2 2 |
| 3 3 3 5     |
---------------
move#16: (7, 'down')
---------------
|     4 2 2   |
|     4 2 2   |
| 5 4 1 1 4  
| 5 4 4 5 4   |
| 5   4 5 2 2 |
| 3 3 3 5     |
---------------
move#17: (13, 'down')
---------------
|     4 2 2   |
|     4 2 2   |
| 5   1 1 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
| 3 3 3 5     |
---------------
move#18: (14, 'left')
---------------
|     4 2 2   |
|     4 2 2   |
| 5 1 1   4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
| 3 3 3 5     |
---------------
move#19: (21, 'up')
---------------
|     4 2 2   |
|     4 2 2   |
| 5 1 1 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
| 3 3 3       |
---------------
move#20: (30, 'right')
---------------
|     4 2 2   |
|     4 2 2   |
| 5 1 1 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
|   3 3 3     |
---------------
move#21: (31, 'right')
---------------
|     4 2 2   |
|     4 2 2   |
| 5 1 1 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
|     3 3 3   |
---------------
move#22: (32, 'right')
---------------
|     4 2 2   |
|     4 2 2   |
| 5 1 1 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
|       3 3 3 |
---------------
move#23: (20, 'down')
---------------
|     4 2 2   |
|     4 2 2   |
| 5 1 1 5 4  
| 5 4   5 4   |
| 5 4 4 5 2 2 |
|     4 3 3 3 |
---------------
move#24: (12, 'down')
---------------
|     4 2 2   |
|     4 2 2   |
|   1 1 5 4  
| 5 4   5 4   |
| 5 4 4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#25: (13, 'left')
---------------
|     4 2 2   |
|     4 2 2   |
| 1 1   5 4  
| 5 4   5 4   |
| 5 4 4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#26: (2, 'down')
---------------
|       2 2   |
|     4 2 2   |
| 1 1 4 5 4  
| 5 4   5 4   |
| 5 4 4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#27: (8, 'down')
---------------
|       2 2   |
|       2 2   |
| 1 1 4 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#28: (9, 'left')
---------------
|       2 2   |
|     2 2     |
| 1 1 4 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#29: (8, 'left')
---------------
|       2 2   |
|   2 2       |
| 1 1 4 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#30: (7, 'left')
---------------
|       2 2   |
| 2 2         |
| 1 1 4 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#31: (3, 'left')
---------------
|     2 2     |
| 2 2         |
| 1 1 4 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#32: (2, 'left')
---------------
|   2 2       |
| 2 2         |
| 1 1 4 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#33: (1, 'left')
---------------
| 2 2         |
| 2 2         |
| 1 1 4 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#34: (14, 'up')
---------------
| 2 2         |
| 2 2 4       |
| 1 1 4 5 4  
| 5 4   5 4   |
| 5 4 4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#35: (8, 'up')
---------------
| 2 2 4       |
| 2 2 4       |
| 1 1   5 4  
| 5 4   5 4   |
| 5 4 4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#36: (12, 'right')
---------------
| 2 2 4       |
| 2 2 4       |
|   1 1 5 4  
| 5 4   5 4   |
| 5 4 4 5 2 2 |
| 5   4 3 3 3 |
---------------
move#37: (18, 'up')
---------------
| 2 2 4       |
| 2 2 4       |
| 5 1 1 5 4  
| 5 4   5 4   |
| 5 4 4 5 2 2 |
|     4 3 3 3 |
---------------
move#38: (26, 'up')
---------------
| 2 2 4       |
| 2 2 4       |
| 5 1 1 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
|       3 3 3 |
---------------
move#39: (33, 'left')
---------------
| 2 2 4       |
| 2 2 4       |
| 5 1 1 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
|     3 3 3   |
---------------
move#40: (32, 'left')
---------------
| 2 2 4       |
| 2 2 4       |
| 5 1 1 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
|   3 3 3     |
---------------
move#41: (31, 'left')
---------------
| 2 2 4       |
| 2 2 4       |
| 5 1 1 5 4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
| 3 3 3       |
---------------
move#42: (15, 'down')
---------------
| 2 2 4       |
| 2 2 4       |
| 5 1 1   4  
| 5 4 4 5 4   |
| 5 4 4 5 2 2 |
| 3 3 3 5     |
---------------
move#43: (16, 'up')
---------------
| 2 2 4       |
| 2 2 4   4   |
| 5 1 1   4  
| 5 4 4 5     |
| 5 4 4 5 2 2 |
| 3 3 3 5     |
---------------
move#44: (10, 'up')
---------------
| 2 2 4   4   |
| 2 2 4   4   |
| 5 1 1      
| 5 4 4 5     |
| 5 4 4 5 2 2 |
| 3 3 3 5     |
---------------
move#45: (13, 'right')
---------------
| 2 2 4   4   |
| 2 2 4   4   |
| 5   1 1    
| 5 4 4 5     |
| 5 4 4 5 2 2 |
| 3 3 3 5     |
---------------
move#46: (14, 'right')
---------------
| 2 2 4   4   |
| 2 2 4   4   |
| 5     1 1  
| 5 4 4 5     |
| 5 4 4 5 2 2 |
| 3 3 3 5     |
---------------
move#47: (15, 'right')
---------------
| 2 2 4   4   |
| 2 2 4   4   |
| 5       1 1
| 5 4 4 5     |
| 5 4 4 5 2 2 |
| 3 3 3 5     |
---------------
Note: the index of each brick
 0 = space
 1 = vertical target brick of length 2 
 2 = horizontal brick of length 2
 4 = vertical   brick of length 2
 3 = horizontal brick of length 2
 5 = vertical   brick of length 3
```
