# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Define the package as scipy.linalg import lu.
2. Get input from user and print L and U matrix by 'print' .
3. Define a package as "from scipy.linalg import lu_factor, lu_solve" and create the variable as 'X' include the package in that variable
4. print the variable 'X'

## Program:
(i) To find the L and U matrix
```
/*
'''Program to find L and U matrix using LU decomposition.
Developed by: Vemareddygari Pallavi
RegisterNumber: 212225230293
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np 
from scipy.linalg import lu
matrix = np.array(eval(input()))
P,L,U=lu(matrix)
print(L)
print(U)

*/
```
(ii) To find the LU Decomposition of a matrix
```
/*
'''Program to solve a matrix using LU decomposition.
Developed by: Vemareddygari Pallavi
RegisterNumber: 212225230293
'''
# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix=np.array(eval(input()))
constant=np.array(eval(input()))
piv,lu=lu_factor(matrix)
result=lu_solve((piv,lu),constant)
print(result)
*/
```

## Output:
<img width="884" height="844" alt="image" src="https://github.com/user-attachments/assets/f6d533bd-33e5-430a-87ad-4e0d7a74f0f8" />

<img width="827" height="744" alt="image" src="https://github.com/user-attachments/assets/43e38a76-0df1-47a4-8b3a-65940fa4ce47" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

