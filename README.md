print("Here we will generate your report card")
print("You will enter your name and we will calculate your report card")
def calculate_grade(average):
    if average >=90:
        return "A+"
    if average >=80:
        return "A"
    if average >=70:
        return "B"
    if average >=60:
        return "C"
    if average >=50:
        return "D"
    else:
        return "F"
student1= input("Enter your name")
subjects = ["Math", "Science", "Hindi", "Social Studies","English"]
marks = {}
for subject in subjects:
    marks[subject] = int(input(f"Enter your marks for {subject}"))

total = sum(marks.values())
average = total / len(subjects)
grade = calculate_grade(average)
print("\n ----Report Card----")
print(f"Hello {student1},Your total was {total}")
print(f"Your average was {average}")
print(f"and your grade was {grade}")
