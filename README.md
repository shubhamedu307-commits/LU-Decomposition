# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2.Import the necessary libraries(numpy,scipy.linalg)
3.Define the matrix using numpy
4.Use lu(),lu_solve(),lu_factor() to get the solutions
5.End the program 

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: SHUBHAM KUMAR
RegisterNumber: 26013866
*/
```
```
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"


import numpy as np 

from scipy.linalg import lu

A=np.array(eval(input()))
P,L,U = lu(A)
print(L)
 
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: SHUBHAM KUMAR
RegisterNumber: 26013866
*/
```
```
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"


import numpy as np
from scipy.linalg import lu_factor, lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot=lu_factor(A)

x=lu_solve((lu,pivot),B)

print(x)
```

## Output:

<img width="1462" height="618" alt="Exp-05 -A Record-LU Decomposition" src="https://github.com/user-attachments/assets/f54fead4-e5a0-4acd-bf22-849a502b2537" />

<img width="835" height="291" alt="Exp-05 - A Record-LU Decomposition result" src="https://github.com/user-attachments/assets/093a0e80-12c7-4641-b229-7633715283a8" />

<img width="615" height="517" alt="Exp-05 - B Record-LU Decomposition" src="https://github.com/user-attachments/assets/15dcee06-c772-4ded-a531-a220c0a74708" />

<img width="581" height="121" alt="Exp-05 -B Record-LU Decomposition RESULT" src="https://github.com/user-attachments/assets/785e7495-5e7f-40d6-86c0-75dfc359f043" />







## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

