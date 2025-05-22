# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```python
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Mukesh R
RegisterNumber: 212224240098

import numpy as np
import matplotlib.pyplot as plt
x=np.array(eval(input()))
y=np.array(eval(input()))
x_mean=np.mean(x)
y_mean=np.mean(y)
print(x_mean)
print(y_mean)
num,denom = 0,0
for i in range(len(x)):
  num+=((x[i]-x_mean)*(y[i]-y_mean))
  denom+=(x[i]-x_mean)**2
m=num/denom
b=y_mean-m*x_mean
print(m,b)
y_predicted=m*x+b 
y_predicted
plt.scatter(x,y,color='black')
plt.plot(x,y_predicted,color='black')
plt.show()
print(m*3+b)

*/
```

## Output:
![image](https://github.com/user-attachments/assets/62ea6836-8826-4649-b100-002cde3ccefc)

![image](https://github.com/user-attachments/assets/93b59c2a-2168-4ff6-860a-34725bece086)

![image](https://github.com/user-attachments/assets/4ac5e3d1-cf4d-469c-b619-0bf49cb195f7)

![image](https://github.com/user-attachments/assets/6170b40f-7c70-40de-8a2e-99b90cec3244)

![image](https://github.com/user-attachments/assets/c43372ff-23ba-4416-a7de-ec1ee82f3f09)







## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
