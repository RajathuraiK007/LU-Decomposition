# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Define the matrix using numpy
4. Use lu(),lu_solve(),lu_factor() to get the solutions
5. End the program

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Rajathurai K
RegisterNumber: 212225100036
*/
import numpy as np
from scipy.linalg import lu
matrix=np.array(eval(input()))
P, L, U = lu(matrix)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Rajathurai K
RegisterNumber: 212225100036
*/
import numpy as np
from scipy.linalg import lu_factor, lu_solve
matrix=np.array(eval(input()))
constant=np.array(eval(input()))
piv, lu = lu_factor(matrix)
result = lu_solve((piv,lu),constant)
print(result)
```

## Output:



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

