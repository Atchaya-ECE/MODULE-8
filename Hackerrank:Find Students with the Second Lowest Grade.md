# 🎓 Hackerrank:Python Program to Find Students with the Second Lowest Grade

This program reads student names and their corresponding grades, identifies the *second lowest grade, and prints the names of all students who have that grade in **alphabetical order*.

---

## 🎯 Aim

To write a Python program to:
- Read a list of students and their grades.
- Identify the second lowest grade.
- Print the names of students who have that grade, sorted alphabetically.

---

## 🧠 Algorithm

1. *Read* an integer n representing the number of students.
2. *Read* each student’s name and grade, and store them as a sublist inside a list.
3. *Extract* all the grades and sort them.
4. *Identify* the second lowest grade from the sorted grade list.
5. *Collect* names of all students whose grade matches the second lowest grade.
6. *Sort* the names alphabetically.
7. *Print* each name on a new line.

---

## 💻  Program

l1=[]
l2=[]
for _ in range(int(input())):
   name = input()
   score = float(input())
   l1.extend([name,score])
   l2.append(l1)
   l1=[]
l3=[]
l4=[]
for i in l2:
  l3.append(i[1])
l3.sort()
for i in l2:
  if i[1]==l3[1]:
     l4.append(i[0])
l4.sort()
for i in l4:
  print(i)


## Output
![image](https://github.com/user-attachments/assets/9449f4da-1beb-4561-a55b-e6abb641834a)

## Result
Thus the program has been successfully executed
