# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Read the elements of augmented matrix into array A and B
2. Calculate elements of L and U
3. print L and U matrix
4. Find V by solving LV=B by forword substitution
5. Find X by solving UX=V by backward substitution
6. print array X as the solution
8. 

## Program:
(i) To find the L and U matrix
```python
'''Program to find L and U matrix using LU decomposition.
Developed by: Nithish D.M
RegisterNumber: 23009587
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
```python
'''Program to solve a matrix using LU decomposition.
Developed by: Nithish D.M
RegisterNumber: 23009587
'''
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
(i) To find the L and U matrix
![Screenshot from 2023-12-27 10-33-19](https://github.com/Mrnithishx/LU-Decomposition/assets/148201573/eb6f14f0-04bb-4d78-b8af-b64ce18aa502)

(ii) To find the LU Decomposition of a matrix
![Screenshot from 2023-12-27 10-35-02](https://github.com/Mrnithishx/LU-Decomposition/assets/148201573/a326b4e6-cd10-403c-b727-d4388850a615)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

