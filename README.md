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

### Question 4 – Internal and External Marks
## The internal and external examination marks of five students are stored in two NumPy arrays. Write a program to calculate the final marks of each student using NumPy array operations. 
```

import numpy as np

internal = np.array([20, 18, 22, 16, 19])
external = np.array([65, 72, 60, 70, 68])

final_marks = internal + external

print("Internal marks:", internal)
print("External marks:", external)
print("Final marks:", final_marks)

```
## output:

<img width="1481" height="308" alt="image" src="https://github.com/user-attachments/assets/7bd910b0-5f49-4ded-abf5-7b4c616f6cef" />


### Question 5 – Pass Percentage Analysis
## The marks obtained by five students are [45, 78, 56, 32, 91]. Using NumPy Boolean masking, identify the students who have secured 50 marks or above.
```
import numpy as np

marks = np.array([45, 78, 56, 32, 91])

passed = marks[marks >= 50]

print("Input marks:", marks)
print("Marks 50 or above:", passed)
print("Number of students:", passed.size)


```
## output:
<img width="1515" height="281" alt="image" src="https://github.com/user-attachments/assets/f6d2ed0d-b7e4-4d71-97b7-7fb0830c9719" />




### Question 6 – Average Marks
## The marks of five students in three subjects are represented using a NumPy matrix. Write a program to calculate the average marks of each student.

```

import numpy as np

marks = np.array([
    [78, 85, 90],
    [65, 72, 80],
    [88, 91, 84],
    [56, 62, 70],
    [95, 89, 92]
])

average = np.mean(marks, axis=1)

print("Marks matrix:")
print(marks)
print("Average marks of each student:", average)

```
## output:
<img width="1836" height="466" alt="image" src="https://github.com/user-attachments/assets/f17f8606-e288-4933-be82-8a5459811160" />



### Question 7 – Class Performance Statistics
## The marks obtained by five students are [67, 82, 91, 74, 58]. Using NumPy statistical functions, determine the total, average, highest, lowest, and standard deviation of the marks. 
```
import numpy as np

marks = np.array([67, 82, 91, 74, 58])

print("Input marks:", marks)
print("Total:", np.sum(marks))
print("Average:", np.mean(marks))
print("Highest:", np.max(marks))
print("Lowest:", np.min(marks))
print("Standard deviation:", np.std(marks))


```
## output:
<img width="1692" height="317" alt="image" src="https://github.com/user-attachments/assets/4eb3b741-b770-4c86-be25-415b48124a5c" />




### Question 8 – Subject-wise Performance
## The marks of five students in three subjects are stored in a NumPy matrix. Write a program to calculate the total marks obtained in each subject using an appropriate axis operation.


```
import numpy as np

marks = np.array([
    [78, 85, 90],
    [65, 72, 80],
    [88, 91, 84],
    [56, 62, 70],
    [95, 89, 92]
])

subject_total = np.sum(marks, axis=0)

print("Marks matrix:")
print(marks)
print("Total marks in each subject:", subject_total)


```
## output:

<img width="1672" height="457" alt="image" src="https://github.com/user-attachments/assets/0bf1b09f-e99d-4ab7-ad3a-d15112ca6934" />



### Question 9 – Student-wise Performance
## The marks of five students in three subjects are stored in a NumPy matrix. Write a program to calculate the total marks obtained by each student using an appropriate axis operation.


```
import numpy as np

marks = np.array([
    [78, 85, 90],
    [65, 72, 80],
    [88, 91, 84],
    [56, 62, 70],
    [95, 89, 92]
])

student_total = np.sum(marks, axis=1)

print("Marks matrix:")
print(marks)
print("Total marks of each student:", student_total)


```
## output:
<img width="1682" height="445" alt="image" src="https://github.com/user-attachments/assets/3cf95478-9071-4b87-b26b-c913668a497a" />




### Question 10 – Student Ranking
## The total marks obtained by five students are [245, 278, 219, 290, 256]. Use NumPy sorting and indexing operations to arrange the marks in order and determine the ranking of the students.


```
import numpy as np

marks = np.array([245, 278, 219, 290, 256])

sorted_marks = np.sort(marks)[::-1]
ranking = np.argsort(marks)[::-1]

print("Input total marks:", marks)
print("Marks in descending order:", sorted_marks)
print("Student ranking:", ranking + 1)

for i in range(5):
    print("Rank", i + 1, ": Student", ranking[i] + 1)


```
## output:
<img width="1616" height="395" alt="image" src="https://github.com/user-attachments/assets/6e2822c0-89f2-4a8b-ab5e-a444e1419a1c" />



### Question 11 – Duplicate Marks Analysis
## The marks obtained by five students are [85, 92, 85, 76, 92]. Use NumPy functions to identify the unique marks obtained by the students.

 
```

import numpy as np

marks = np.array([85, 92, 85, 76, 92])

unique_marks = np.unique(marks)

print("Input marks:", marks)
print("Unique marks:", unique_marks)

```
## output:

<img width="1486" height="273" alt="image" src="https://github.com/user-attachments/assets/edf52673-7a16-44f8-b488-f0cc203462e2" />



### Question 12 – Missing Marks
## The marks of five students are represented as [78, 85, np.nan, 92, 67], where np.nan represents a missing mark. Write a NumPy program to calculate the average marks without considering the missing value.


```
import numpy as np

marks = np.array([78, 85, np.nan, 92, 67])

average = np.nanmean(marks)

print("Input marks:", marks)
print("Average without missing value:", average)


```
## output:
<img width="1622" height="282" alt="image" src="https://github.com/user-attachments/assets/be766ce3-41f8-47cc-a28b-5cd804036e94" />




### Question 13 – Grade Classification
## The marks obtained by five students are [95, 82, 74, 61, 45]. Using NumPy conditional operations, classify the students into appropriate grade categories based on their marks.


```
import numpy as np

marks = np.array([95, 82, 74, 61, 45])

grades = np.select(
    [
        marks >= 90,
        marks >= 80,
        marks >= 70,
        marks >= 60
    ],
    [
        "A",
        "B",
        "C",
        "D"
    ],
    default="F"
)

print("Input marks:", marks)
print("Grades:", grades)


```
## output:
<img width="1592" height="622" alt="image" src="https://github.com/user-attachments/assets/9bafbe6d-a846-46d9-980b-ec4b9b06eb37" />




### Question 14 – Random Marks Generation
## Generate marks for five students using NumPy's random number generation functionality. Perform basic statistical analysis on the generated marks.


```
import numpy as np

np.random.seed(10)

marks = np.random.randint(35, 101, size=5)

print("Generated marks:", marks)
print("Total:", np.sum(marks))
print("Average:", np.mean(marks))
print("Highest:", np.max(marks))
print("Lowest:", np.min(marks))


```
## output:
<img width="1486" height="367" alt="image" src="https://github.com/user-attachments/assets/45532a5b-2e30-4224-ab62-17fa1d2909d5" />




### Question 15 – Student Performance Analysis
## The marks of five students in three subjects are stored in a NumPy array. Develop a program to perform a complete student performance analysis by calculating the total marks, average marks, highest marks, lowest marks, and identifying students who perform above the class average.

```
import numpy as np
marks = np.array([
    [78, 85, 90],
    [65, 72, 80],
    [88, 91, 84],
    [56, 62, 70],
    [95, 89, 92]
])
total = np.sum(marks, axis=1)
average = np.mean(marks, axis=1)
highest = np.max(marks, axis=1)
lowest = np.min(marks, axis=1)
class_average = np.mean(total)
above_average = np.where(total > class_average)[0] + 1
print("Marks matrix:")
print(marks)
print("Total marks:", total)
print("Average marks:", average)
print("Highest mark:", highest)
print("Lowest mark:", lowest)
print("Class average total:", class_average)
print("Students above class average:", above_average)

```
## output:
<img width="1843" height="748" alt="image" src="https://github.com/user-attachments/assets/4768f86c-1a84-41ba-85dc-c0364cb28f1e" />

