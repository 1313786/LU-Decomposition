# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

(i) To find the L and U matrix

## Algorithm 

### Step 1: Start the Program

### Step 2: numpy for matrix creation and handling.

### Step 3: scipy.linalg.lu for LU decomposition.

### Step 4: Input the Matrix

### Step 5: Take the square matrix A as input.

### Step 6: Use eval(input()) to allow entry in Python list format (e.g., [[2,3],[4,5]]).

### Step 7: Use lu(A) from SciPy which returns:

(ii) To find the LU Decomposition of a matrix

## Algorithm

### Step 1: Start the Program

### Step 2: numpy for matrix input and handling.

### Step 3: lu_factor and lu_solve from scipy.linalg for LU decomposition and solving.

### Step 4: Input the coefficient matrix A (square matrix).

### Step 5: Input the right-hand side vector or matrix B.

### Step 6: Use lu_factor(A) to compute:

LU: combined LU decomposition matrix,

PV: pivot indices for row permutations.

### Step 7: Use lu_solve((PV, LU), B) to solve the system Ax = B.

### Step 8: Output the result vector x which solves Ax = B.
## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: IRFAN KHAN.N
RegisterNumber: 212224230097
'''
import numpy as np 
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: IRFAN KHAN.N
RegisterNumber: 212224230097
'''
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
piv,lu=lu_factor(A)
result=lu_solve((piv,lu),B)
print(result)
```

## Output:

(i) To find the L and U matrix
![Screenshot 2025-05-13 172555](https://github.com/user-attachments/assets/26ab573d-81d1-42b8-9b74-87814593af50)

(ii) To find the LU Decomposition of a matrix

![Screenshot 2025-05-13 172607](https://github.com/user-attachments/assets/e260ce13-bdeb-4f3a-8489-89b435fe06a5)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

