# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### (i) To find the L and U matrix using LU decomposition:

### Algorithm Steps:

1. Import the necessary libraries (scipy.linalg and numpy).

2. Accept a matrix as input from the user.

3. Convert the input matrix into a NumPy array.

4. Use the LU decomposition function (lu) from scipy.linalg to decompose the matrix into the product of a permutation matrix P, a lower triangular matrix L, and an upper triangular matrix U.

5. Print the lower triangular matrix L.

6. Print the upper triangular matrix U.


### (ii) To find the LU Decomposition of a matrix:

### Algorithm Steps:

1. Import the necessary libraries (scipy.linalg and numpy).
   
2. Accept a matrix as input from the user.

3. Convert the input matrix into a NumPy array.

4. Accept a constant matrix (right-hand side of the equations) as input from the user.

5. Convert the constant matrix into a NumPy array.

6. Use the LU factorization function (lu_factor) from scipy.linalg to compute the LU decomposition of the coefficient matrix.

7. Use the LU solve function (lu_solve) to find the solution to the system of linear equations.

8. Print the solution matrix.
## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: K.Madhava Reddy
RegisterNumber: 23009929
'''
from scipy.linalg import lu
import numpy as np
arr=eval(input())
A=np.array(arr)
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: K.Madhava Reddy
RegisterNumber: 23009929
'''

# To print X matrix (solution to the equations)
from scipy.linalg import lu_factor,lu_solve
import numpy as np
arr=eval(input())
constant=eval(input())
A=np.array(arr)
B=np.array(constant)
result=lu_factor(A)
solution=lu_solve(result,B)
print(solution)
```

## Output:
(i)

![image](https://github.com/Madhavareddy09/LU-Decomposition/assets/145742470/bf007a46-6fbf-4bc3-8dd6-dbe95e834468)


(ii)
![image](https://github.com/Madhavareddy09/LU-Decomposition/assets/145742470/4b11dd49-ce8a-4d83-8ea0-2ffdcdf4ab8f)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

