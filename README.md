# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import required libraries numpy and scipy.linalg.
2. Input the matrix/matrices using eval(input()).
3. Perform LU decomposition using lu().
4. Print the results L and U matrices or solution X matrix

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: HARSHIDA K S
RegisterNumber: 212224040108
'''
import numpy as np
from scipy.linalg import lu
a=eval(input())
b=np.array(a,dtype=float)
p,l,u=lu(b)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: HARSHIDA K S
RegisterNumber: 212224040108
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu,solve
a=np.array(eval(input()))
b=np.array(eval(input()))
p,l,u=lu(a)
pb=p @ b
y=solve(l,pb,lower=True)
x=solve(u,y)
print(x)

```

## Output:

(i) To find the L and U matrix

<img width="1275" height="823" alt="exp5(1)" src="https://github.com/user-attachments/assets/6606bb39-8d95-4655-af22-74887b5ab347" />

(ii) To find the LU Decomposition of a matrix

<img width="1260" height="707" alt="exp5(2)" src="https://github.com/user-attachments/assets/b9ef082f-6a92-4408-a775-084339e1acad" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

