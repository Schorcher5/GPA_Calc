# GPA_Calc
This is a very limited GPA calculator I made using python. Looking to recieve feedback on my code.
class GPA:
    
    def __init__(self, classes):
        GPA.classes = classes
    
    #Converts letter grade and credit into a value that can be added to the GPA
   
    def gpa(credit,grade,counter):
        credit /= 3
        if grade[counter] == "A":
            credit *= 4.0
        elif grade[counter] == "+A":
            credit *= 4.33
        elif grade[counter] == "-A":
            credit *= 3.67
        elif grade[counter] == "+B":
            credit *= 3.33
        elif grade[counter] == "B":
            credit *= 3.0
        elif grade[counter] == "-B":
            credit *= 2.67
        elif grade[counter] == "+C":
            credit *= 2.33
        elif grade[counter] == "C":
            credit *= 2.0
        elif grade[counter] == "-C":
            credit *= 1.67
        elif grade[counter] == "D":
            credit *= 1.0
        elif grade[counter] == "F":
            credit *= 0.0
        
        return credit
        
        #This diveds the total score and asks for the credit value and letter grade
       
    def credits(self):
        credits = []
        grade = []
        counter = 1
        while counter <= self.classes:
            credits.append(int(input("How many credits? ")))
            letter_grade =input("What was your letter grade? ")
            grade.append(letter_grade.upper())
            counter += 1
        counter = 0
        total = 0.0
        for credit in credits:
            total += GPA.gpa(credit,grade,counter)
           
            counter += 1
        total /= (counter)
        print(total)

number_of_classes = input(int("How many classes did you take?:  "))
answer = GPA(number_of_classes)
answer.credits()
