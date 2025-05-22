## NAME: DEEPIKA P
## REGISTER NO: 212223240024
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
## Output:
(i) To find the L and U matrix
![Screenshot 2025-05-14 143808](https://github.com/user-attachments/assets/0cfadc7f-377d-453f-9812-cbec4ce1fc36)

## Algorithm:
Step 1: Start the program.

Step 2: Input the matrix A and vector b.

Prompt the user to enter a square matrix A (as a list of lists).

Prompt the user to enter a column vector b (as a list).

Step 3: Convert inputs to NumPy arrays.

Use np.array() to convert the input matrix A and vector b to NumPy arrays.

Step 4: Perform LU decomposition.

Use lu_factor(A) from scipy.linalg to compute the LU decomposition of matrix A.

This returns:

lu: the combined LU decomposition matrix.

piv: pivot indices representing the row permutations.

Step 5: Solve the system of linear equations Ax = b.

Use lu_solve((lu, piv), b) to solve for x.

Step 6: Print the solution x.

Step 7: End the program.
## Program:
(ii) To find the LU Decomposition of a matrix
import numpy as np\
from scipy.linalg import lu_factor, lu_solve\
A = np.array(eval(input()))\
b = np.array(eval(input()))\
lu, piv = lu_factor(A)\
X = lu_solve((lu, piv),b)\
print(X)
## Output:
(ii) To find the LU Decomposition of a matrix
![Screenshot 2025-05-14 143930](https://github.com/user-attachments/assets/13ec8add-03ea-44e2-b131-3811941375bd)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

