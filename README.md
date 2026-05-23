# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Write a python program for the given matrix.
2.Using numpy library.
3.Using the np.linalg.matrix_rank(),we can find the rank of the matrix.
4.Run the program and get the output.

## Program:
```
'''Program to find L and U matrix using LU decomposition.
Developed by: ROHITH R
RegisterNumber: 21225230229
'''
import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"
import numpy as np
from scipy.linalg import lu
matrix = eval(input())
P,L,U = lu(matrix)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: ROHITH R
RegisterNumber: 212225230229
'''
import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array([[3,2,7],[2,3,1,],[3,4,1]])
B=np.array([4,5,7])
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),B)
print(x)


```

## Output:
<img width="927" height="787" alt="image" src="https://github.com/user-attachments/assets/89ed3acc-fef8-457b-ad97-de1890b96954" />


<img width="717" height="548" alt="image" src="https://github.com/user-attachments/assets/8f7d0ffa-f121-4e5b-a930-2124488cde09" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

