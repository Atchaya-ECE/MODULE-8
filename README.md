# # 🔢 Hackerrank:# 🏆 Student Topper Finder

This Python program helps determine the *top-performing student* based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

## 🎯 Aim

To maintain a dictionary of students with their marks in five subjects, calculate their *total marks, store them in a new dictionary, and identify the **student with the highest total (topper)*.

---

## 🧠 Algorithm

1. *Start* the program.
2. Create a dictionary student_marks:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary total_marks.
4. Loop through student_marks:
   - Calculate the total marks using sum().
   - Store the result in total_marks.
5. Use max() on total_marks to find the student with the highest total.
6. Print:
   - The total_marks dictionary.
   - The *topper's name and score*.

---

## 💻 PROGRAM:

student_marks = {
    "Alice": [88, 76, 92, 85, 79],
    "Bob": [90, 91, 85, 88, 92],
    "Charlie": [70, 80, 75, 65, 72],
    "Diana": [95, 89, 94, 90, 96]
}
total_marks = {}
for student, marks in student_marks.items():
    total_marks[student] = sum(marks)
topper = max(total_marks, key=total_marks.get)
top_score = total_marks[topper]
print("Total Marks of Students:")
for student, total in total_marks.items():
    print(f"{student}: {total}")

print(f"\nTopper: {topper} with {top_score} marks.")

## OUTPUT

Total Marks of Students:
Alice: 420
Bob: 446
Charlie: 362
Diana: 464

Topper: Diana with 464 marks.

## RESULT
Hence Calculated total marks for students and find the topper.

# EXP 37 Hackerrank :   Python Word Wrap Function

This Python program defines a function that *wraps a long string into multiple lines*, ensuring each line does not exceed a specified width.


## Aim

To write a Python function that takes a long string and a specified width, and returns the string formatted with line breaks such that each line has *at most the given width*.


##  Algorithm

1. *Start* the program.
2. Define a function wrap(string, max_width):
   - Create an empty list wrapped_lines to store parts of the string.
   - Loop through the string using steps of max_width.
   - In each iteration, extract a substring of length max_width.
   - Append this substring to the list.
3. Join the list with \n to create the final string.
4. Return the result.
5. *End* the program.




##  Program

def wrap(string, max_width):
    wrapped_lines = []
    for i in range(0, len(string), max_width):
        wrapped_lines.append(string[i:i+max_width])
    return '\n'.join(wrapped_lines)

string = input()
max_width = int(input())
print(wrap(string, max_width))


## Output
![image](https://github.com/user-attachments/assets/59a64531-25ee-4452-a4f5-decdc2dbfb34)

## Result
Thus, the program is verified successfully.

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

# 🏆 Hackerrank:Runner-Up Score Finder in Python

## 🎯 AIM:
To write a Python program that takes a list of scores from participants and finds the *runner-up score* (i.e., the second-highest score), eliminating any duplicates.

---

## 🧠 ALGORITHM:

1. *Start*
2. Create a variable n and get its value from the user (number of participants)
3. Read the list of n scores from the user using input().split() and convert them to integers
4. Store the scores in a list
5. Use set() to remove any duplicate scores
6. Convert the set back to a list and sort it in ascending order
7. Print the second-last element of the sorted list (i.e., the runner-up score)
8. *Stop*

---

## 💻 PROGRAM:

n = int(input("Enter the number of participants: "))
scores = list(map(int, input("Enter the scores separated by space: ").split()))
unique_scores = sorted(set(scores))
if len(unique_scores) < 2:
    print("Runner-up score not available.")
else:
    print("Runner-up score:", unique_scores[-2])


## OUTPUT

Enter the number of participants: 5
Enter the scores separated by space: 2 3 6 6 5
Runner-up score: 5

## RESULT
Hence Found the Runner up score

# 🔍 Hackerrank:Python Program to Check if a String Ends with a Numeric Digit

This Python program checks whether the last character of a given input string is a *numeric digit (0–9)*.

---

## 🎯 Aim

To write a Python program that checks if a given string ends with a number using Python's built-in string methods.

---

## 🧠 Algorithm

1. *Start the program.*
2. *Input* a string from the user.
3. *Access* the last character using indexing (string[-1]).
4. *Check* if the last character is a digit using the .isdigit() method.
5. *If true*, print that the string ends with a number.
6. *Else*, print that the string does not end with a number.
7. *End the program.*

---

## 💻  Program

import re

s = input()
p = '[a-zA-Z0-9]*[0-9]+'
x = re.match(p, s)

if x:
    print("True")
else:
    print("False")

## Output
![image](https://github.com/user-attachments/assets/7ddc3249-b794-4293-8464-501b03bb0a3c)

## Result
Thus the program has been successfully executed
