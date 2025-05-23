# # 🔢 Hackerrank:# 🏆 Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

## 🎯 Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.

---

## 💻 PROGRAM:
```
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
```
## OUTPUT
```
Total Marks of Students:
Alice: 420
Bob: 446
Charlie: 362
Diana: 464

Topper: Diana with 464 marks.
```
## RESULT
Hence Calculated total marks for students and find the topper.
