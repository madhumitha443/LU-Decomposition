# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. FINDING THE 'L' AND 'U' MATRIX : STEP1 : Import the numpy module to use the built-in functions for calculation.

STEP1 : Prepare the lists from each linear equations and assign in np.array().

STEP2 : Using the P,L,U =lu(), we get two results (first is L and second is U) of the given matrix.

STEP3 : end the program

2.FINDING DECOMPOSITION OF THE MATRIX:

STEP1 : Import the numpy module to use the built-in functions for calculation.

STEP2 : Prepare the lists from each linear equations and assign in np.array().

STEP3 : Using the pivot=lu_factor(A) andx=lu_solve((lu,pivot),B) , we can find results the LU Decomposition of a matrix

STEP4 : end the program


## Program:
(i) To find the L and U matrix
~~~
/*
Program to find the L and U matrix.
Developed by: MADHUMITHA R
RegisterNumber: 212225230158
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu 
matrix=np.array(eval(input()))
P,L,U=lu(matrix)
print(L)
print(U)
~~~
(ii) To find the LU Decomposition of a matrix
~~~
/*
Program to find the LU Decomposition of a matrix.
Developed by: MADHUMITHA R
RegisterNumber: 212225230158
*/
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = np.array(eval(input()))
B = np.array(eval(input()))
lu,piv = lu_factor(A)
X = lu_solve((lu,piv),B)
print(X)


## Output:
![alt text](image.png)
![alt text](image-1.png)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

