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
Developed by: Santhan Kumar
RegisterNumber: 23004568
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
Developed by: Santhan Kumar
RegisterNumber: 23004568
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

![image](https://github.com/SANTHAN-2006/LU-Decomposition/assets/80164014/4353b6cd-05ba-481f-a5d7-c93684167011)

(ii)

![image](https://github.com/SANTHAN-2006/LU-Decomposition/assets/80164014/d6e04c8d-fedb-459f-8d51-f1a99e617802)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

