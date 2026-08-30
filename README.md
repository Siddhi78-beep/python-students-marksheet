# python-students-marksheet
print("===== STUDENT MARKSHEET =====")

name = input("Enter student name: ")
roll_no = input("Enter roll number: ")

english = float(input("Enter English marks: "))
maths = float(input("Enter Maths marks: "))
science = float(input("Enter Science marks: "))
computer = float(input("Enter Computer marks: "))
history = float(input("Enter History marks: "))

total = english + maths + science + computer + history
percentage = total / 5

if percentage >= 75:
    grade = "A"
elif percentage >= 60:
    grade = "B"
elif percentage >= 50:
    grade = "C"
elif percentage >= 35:
    grade = "D"
else:
    grade = "F"

print("\n===== MARKSHEET =====")
print("Name:", name)
print("Roll No:", roll_no)
print("English:", english)
print("Maths:", maths)
print("Science:", science)
print("Computer:", computer)
print("History:", history)
print("Total Marks:", total, "/ 500")
print("Percentage:", percentage, "%")
print("Grade:", grade)

if percentage >= 35:
    print("Result: PASS")
else:
    print("Result: FAIL")