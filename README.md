# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the Python program and import the required libraries (NumPy and SciPy).

2. Define the matrix you want to decompose using np.array().

3. Use the lu() function from scipy.linalg to compute the LU decomposition.

4. Display the permutation matrix P, lower triangular matrix L, and upper triangular matrix U.

## Program:
(i) To find the L and U matrix
 import numpy as np\
from scipy.linalg import lu\
A = np.array(eval(input()))\
P,L,U=lu(A)\
print(L)\
print(U)\
(ii) To find the LU Decomposition of a matrix
import numpy as np\
from scipy.linalg import lu_factor, lu_solve\
A = np.array(eval(input()))\
b = np.array(eval(input()))\
lu, piv = lu_factor(A)\
X = lu_solve((lu, piv),b)\
print(X)
## Output:
(i) To find the L and U matrix
![Screenshot 2025-05-14 143808](https://github.com/user-attachments/assets/0cfadc7f-377d-453f-9812-cbec4ce1fc36)
(ii) To find the LU Decomposition of a matrix
![Screenshot 2025-05-14 143930](https://github.com/user-attachments/assets/13ec8add-03ea-44e2-b131-3811941375bd)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

