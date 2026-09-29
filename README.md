# HCL
### Question 1 – Student Marks Array
## The marks obtained by five students in a subject are given as [78, 65, 89, 56, 92]. Create a NumPy array and display the array along with its basic properties.
```
import numpy as np
marks = np.array([78, 65, 89, 56, 92])
print("Input marks:", marks)
print("Number of elements:", marks.size)
print("Shape:", marks.shape)
print("Data type:", marks.dtype)
print("Number of dimensions:", marks.ndim)
```

## output:
<img width="1566" height="317" alt="image" src="https://github.com/user-attachments/assets/0e02aa3b-4cb2-41e6-9626-c960d1f4e3e4" />

### Question 2 – Student Marks Access
## The marks of five students are stored in a NumPy array as [72, 85, 64, 90, 76]. Write a program to access and display specific student marks using NumPy indexing and slicing.
```
import numpy as np
marks = np.array([72, 85, 64, 90, 76])
print("Input marks:", marks)
print("First student:", marks[0])
print("Third student:", marks[2])
print("Last student:", marks[-1])
print("First three students:", marks[:3])
print("Students 2 to 4:", marks[1:4])

```
## output:
<img width="1531" height="320" alt="image" src="https://github.com/user-attachments/assets/f83a3d13-67bb-4003-8cab-dd8a01934bec" />



### Question 3 – Subject-wise Marks
## The marks obtained by five students in three subjects are given below.
  Create a NumPy array to represent the data and reshape it into an appropriate matrix format.[78, 85, 90, 65, 72, 80, 88, 91, 84, 56, 62, 70, 95, 89, 92]
```
import numpy as np
marks = np.array([78, 85, 90, 65, 72, 80, 88, 91, 84,
                  56, 62, 70, 95, 89, 92])
matrix = marks.reshape(5, 3)
print("Input data:", marks)
print("Marks matrix:")
print(matrix)

```
## output:
<img width="1770" height="318" alt="image" src="https://github.com/user-attachments/assets/4a57fd0c-3a67-4722-918f-cfd4c8e4b4a0" />

###
## 
```



```
## output:


### Question 4 – Internal and External Marks
## The internal and external examination marks of five students are stored in two NumPy arrays. Write a program to calculate the final marks of each student using NumPy array operations. 
```



```
## output:



### Question 5 – Pass Percentage Analysis
## The marks obtained by five students are [45, 78, 56, 32, 91]. Using NumPy Boolean masking, identify the students who have secured 50 marks or above.
```



```
## output:




### Question 6 – Average Marks
## The marks of five students in three subjects are represented using a NumPy matrix. Write a program to calculate the average marks of each student.

```



```
## output:



### Question 7 – Class Performance Statistics
## The marks obtained by five students are [67, 82, 91, 74, 58]. Using NumPy statistical functions, determine the total, average, highest, lowest, and standard deviation of the marks. 
```



```
## output:




### Question 8 – Subject-wise Performance
## The marks of five students in three subjects are stored in a NumPy matrix. Write a program to calculate the total marks obtained in each subject using an appropriate axis operation.


```



```
## output:




### Question 9 – Student-wise Performance
## The marks of five students in three subjects are stored in a NumPy matrix. Write a program to calculate the total marks obtained by each student using an appropriate axis operation.


```



```
## output:




### Question 10 – Student Ranking
## The total marks obtained by five students are [245, 278, 219, 290, 256]. Use NumPy sorting and indexing operations to arrange the marks in order and determine the ranking of the students.


```



```
## output:



### Question 11 – Duplicate Marks Analysis
## The marks obtained by five students are [85, 92, 85, 76, 92]. Use NumPy functions to identify the unique marks obtained by the students.

 
```



```
## output:




### Question 12 – Missing Marks
## The marks of five students are represented as [78, 85, np.nan, 92, 67], where np.nan represents a missing mark. Write a NumPy program to calculate the average marks without considering the missing value.


```



```
## output:




### Question 13 – Grade Classification
## The marks obtained by five students are [95, 82, 74, 61, 45]. Using NumPy conditional operations, classify the students into appropriate grade categories based on their marks.


```



```
## output:




### Question 14 – Random Marks Generation
## Generate marks for five students using NumPy's random number generation functionality. Perform basic statistical analysis on the generated marks.


```



```
## output:




### Question 15 – Student Performance Analysis
## The marks of five students in three subjects are stored in a NumPy array. Develop a program to perform a complete student performance analysis by calculating the total marks, average marks, highest marks, lowest marks, and identifying students who perform above the class average.

```



```
## output:
