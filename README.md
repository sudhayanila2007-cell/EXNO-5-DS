# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import pandas as pd 
import numpy as np 
import matplotlib.pyplot as plt
```
# Line Plot:
```
marks=[13,45,63,78] 
student=['ABC','QOR','EFB','TOB'] 
plt.plot(marks,student) 
plt.xlabel('Marks') 
plt.ylabel('Student name') 
plt.show()
```
<img width="1129" height="555" alt="Screenshot 2026-08-25 151617" src="https://github.com/user-attachments/assets/98823bb5-5b66-4864-a917-b93e8aa979ce" />

```
student=['A','B','C','D'] 
attendence=[90,85,73,88] 
plt.plot(attendence,student) 
plt.xlabel('Attendence') 
plt.ylabel('Student name') 
plt.show()
```
<img width="1097" height="552" alt="Screenshot 2026-08-25 151630" src="https://github.com/user-attachments/assets/d6b0a6d8-1a14-4094-a925-564c51cb90ab" />

# Scatter Plot:
```
x=[10,20,30,40,50] 
y=[100,200,300,400,500] 
plt.scatter(x,y,label='stars',color='green',marker='*',s=30) 
plt.show()
```
<img width="1031" height="533" alt="Screenshot 2026-08-25 151642" src="https://github.com/user-attachments/assets/2b97e185-cc82-4989-a623-99606c27f26d" />

```
x=np.arange(0,15) 
y=np.arange(0,15) 
x 
y 
plt.scatter(x,y,c='r') 
plt.xlabel('X axis') 
plt.ylabel('y axis') 
plt.title('Scatter plot') 
plt.show()
```
<img width="1031" height="574" alt="Screenshot 2026-08-25 151651" src="https://github.com/user-attachments/assets/b624dadd-f46a-42e0-8fd8-987fc2c11bd7" />

# Pie Chart:
```
act=['eat','sleep','work','play'] 
slices=[3,7,8,6] 
color=['r','y','g','b'] 
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%') 
plt.legend() 
plt.show()
```
<img width="1165" height="537" alt="Screenshot 2026-08-25 151702" src="https://github.com/user-attachments/assets/cd5756fd-ed4f-4d15-9b80-a234b7a4f985" />

```
feedback=['Good','excellent','Perfect','Ok'] 
slices=[4,10,3,8] 
color=['y','r','b','g'] 
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%') 
plt.legend() 
plt.show()
```
<img width="1025" height="518" alt="Screenshot 2026-08-25 151712" src="https://github.com/user-attachments/assets/69c92ab0-aa08-4d17-b862-ddb4236021f3" />

# Area Chart:
```
x = [1, 2, 3, 4, 5] 
y1 = [10, 12, 14, 16, 18] 
y2 = [5, 7, 9, 11, 13] 
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue') 
plt.fill_between(x, y2, color='green') 
plt.plot(x, y1, color='red') 
plt.plot(x, y2, color='black') 
plt.legend(['y1','y2']) 
plt.show()
```
<img width="1186" height="523" alt="Screenshot 2026-08-25 151722" src="https://github.com/user-attachments/assets/64ddf62e-e3b4-4b3f-b74d-98687936ab61" />

# Bar Chart:
```
height = [10, 24, 36, 40, 5] 
names = ['one', 'two', 'three', 'four', 'five'] 
c1=['red', 'green'] 
c2=['b', 'g'] 
plt.bar (names, height, width=0.8, color=c1) 
plt.xlabel('x - axis') 
plt.ylabel('y - axis') 
plt.title('My bar chart!') 
plt.show()
```
<img width="1088" height="581" alt="Screenshot 2026-08-25 151732" src="https://github.com/user-attachments/assets/2acc5bae-5d0e-49be-8d48-e4c3a376b4da" />

# Histogram:
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1] 
plt.hist(x, bins = 10, color='blue', alpha=0.5) 
plt.show()
```
<img width="1091" height="531" alt="Screenshot 2026-08-25 151740" src="https://github.com/user-attachments/assets/40b96acf-1654-418b-9f2b-90f7de1e031c" />

# Box Plot:
```
np.random.seed(0) 
data=np.random.normal(loc=0, scale=1, size=100) 
data
```
<img width="1172" height="443" alt="Screenshot 2026-08-25 151800" src="https://github.com/user-attachments/assets/44555e18-8536-4aa0-a6c8-2ecdfb859757" />

```
fig, ax= plt.subplots() 
ax.boxplot(data) 
ax.set_xlabel('Data') 
ax.set_ylabel('Values') 
ax.set_title('Box Plot')
```
<img width="1159" height="615" alt="Screenshot 2026-08-25 151812" src="https://github.com/user-attachments/assets/5ae38afa-e350-4cc0-891f-5319ad61f674" />

# Result:
 Thus, all the data visualization techniques of matplotlib has been implemented.
