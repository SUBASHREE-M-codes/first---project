# first---project
def input_marks(l):
    n = int(input("Enter number of subjects: "))
    for i in range(n):
        a = int(input("Enter mark in subject: "))
        l.append(a)

def sumavg(l):
    add = sum(l)
    avg = add / len(l)
    return avg

def grading(avg):
    if avg >= 90:
        return "A+ 🌟"
    elif avg >= 75:
        return "A"
    elif avg >= 60:
        return "B"
    elif avg >= 40:
        return "C"
    else:
        return "D - Fail"


l = []
input_marks(l)

avg = sumavg(l)
grade = grading(avg)

print("Your average is:", avg)
print("Your grade is:", grade)