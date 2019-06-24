import matplotlib.pyplot as plt
import pandas as pd

df =  pd.read_csv('student.csv')
#reading data of student.csv file
 
student_names = df["student_name"]
#loading the elements or values of column student_name from student.csv file into variable student_names
Student_marks = df["marks"]
#loading the elements or values of column marks from student.csv file into variable student_marks

explode = (0.1, 0, 0, 0)  
#detaching my name,s data from others

plt.pie(Student_marks, labels=student_names, explode=explode,shadow=True)
#ploting the pie chart

plt.title("Marks obtained by 4 studeents")
#assigning title to the  pie chart

plt.show()
#showing or printing the graph
