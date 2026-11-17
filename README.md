print("===PYTHON TUTORIAL QUIZ===")

print("\nFILL UP YOUR INFORMATION FIRST")

while True:
    name = input("Enter your full name: ").upper()
    if name == "":
        print("NAME CANNOT BE BLANK! Enter your name.")
    else:
        break

while True:
    student_number = input("Enter your student number: ")
    if student_number == "":
        print("STUDENT NUMBER CANNOT BE BLANK! Enter your student number.")
    else:
        break

print("\nWelcome", name)
print("Student Number:", student_number)
print("YOU MAY NOW START THE QUIZ!")


took1 = False
took2 = False
took3 = False
took4 = False
took5 = False
selected_count = 0

while True:
    print("")
    topic_list = ["TOPICS:", "1.Introduction to Programming", "2.Basic Syntax", "3.Arithmetic Operators",
                  "4.If-Else Statements", "5.Loops"]
    print(topic_list[0])
    print(topic_list[1])
    print(topic_list[2])
    print(topic_list[3])
    print(topic_list[4])
    print(topic_list[5])
    print("=====" * 5)


    while True:
        selected_topic = int(input("Enter a topic number (1-5): "))

        if selected_topic < 1 or selected_topic > 5:
            print("Choose only  numbers 1-5!")
            continue

        already_taken = False
        if selected_topic == 1 and took1 == True:
            already_taken = True
        elif selected_topic == 2 and took2 == True:
            already_taken = True
        elif selected_topic == 3 and took3 == True:
            already_taken = True
        elif selected_topic == 4 and took4 == True:
            already_taken = True
        elif selected_topic == 5 and took5 == True:
            already_taken = True

        if already_taken == True:
            print(f"Topic {selected_topic} was already taken! PICK AGAIN.")
            continue

        if selected_topic == 1:
            took1 = True
        elif selected_topic == 2:
            took2 = True
        elif selected_topic == 3:
            took3 = True
        elif selected_topic == 4:
            took4 = True
        elif selected_topic == 5:
            took5 = True

        selected_count = selected_count + 1
        break

    score = 0

    if selected_topic == 1:
        total_quiz = 3
        print("\n")
        print(topic_list[1])
        q1 = "Programming langauge is a special language that computers understand to perform tasks."
        print("\nQ1:", q1)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, because the statement is correct.")

        q2 = "Python was created by Guido van Rossum in 1990 and designed for the beginners."
        print("\nQ2:", q2)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "F":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, because it was created in 1991")

        q3 = "Python is a high-level, easy-to-read programming language."
        print("\nQ3:", q3)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER,because the statement is correct")

    elif selected_topic == 2:
        total_quiz = 4
        print("\n")
        print(topic_list[2])
        q1 = "Python Syntax refers to the set of rules that tells us how to correctly write a program in Python."
        print("\nQ1:", q1)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, because the statement is correct.")

        q2 = "Case Sensitive is that Python treats uppercase & lowercase letters not differently."
        print("\nQ2:", q2)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "F":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, because Case Sensitive is that Python treats uppercase & lowercase letters differently.")

        q3 = "Indentation is required in Python to define blocks of code."
        print("\nQ3:", q3)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, because the statement is correct.")

        q4 = "A variable name can start with a number like: 1name."
        print("\nQ4:", q4)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "F":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, must start with a letter or underscore.")

    elif selected_topic == 3:
        total_quiz = 5
        print("\n")
        print(topic_list[3])
        q1 = "To add two numbers, use the + symbol."
        print("\nQ1:", q1)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, because the statement is correct.")

        q2 = "The - symbol subtracts one number from another."
        print("\nQ2:", q2)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, because the statement is correct.")

        q3 = "* is used for multiplication in Python."
        print("\nQ3:", q3)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, because the statement is correct.")

        q4 = "/ gives the remainder of a division."
        print("\nQ4:", q4)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "F":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, / is division: % is remainder.")

        q5 = "** is used for exponents, example: 2**3=8"
        print("\nQ5:", q5)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, ** means-to the power of")

    elif selected_topic == 4:
        total_quiz = 8
        print("\n")
        print(topic_list[4])
        q1 = "An if block runs only when its condition is True."
        print("\nQ1:", q1)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, because the statement is correct.")

        q2 = "An else block runs when the if condition is True."
        print("\nQ2:", q2)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "F":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, else runs when the condition is false.")

        q3 = "In if-elif-else, Python checks conditions from top to bottom."
        print("\nQ3:", q3)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, checks top first.")

        q4 = "The == symbol means if two values are equal."
        print("\nQ4:", q4)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, == means 'is equal to'.")

        q5 = "The != symbol means 'is not equal to."
        print("\nQ5:", q5)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, != means 'is not equal to'.")

        q6 = "Nested Statement means you cannot put an if statement inside another if statement."
        print("\nQ6:", q6)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "F":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, nested statement you can put an if statement inside another if statement.")

        q7 = "AND means both condition must be True."
        print("\nQ7:", q7)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, because the statement is correct.")

        q8 = "OR means at least ONE condition must be True."
        print("\nQ8:", q8)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, because the statement is correct.")

    elif selected_topic == 5:
        total_quiz = 5
        print("\n")
        print(topic_list[5])
        q1 = "A loop repeats a block of code multiple times."
        print("\nQ1:", q1)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, because the statement is correct.")


        q2 = "A 'for loop' repeats a fixed number of times."
        print("\nQ2:", q2)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, because the statement is correct.")

        q3 = "A 'while loop' repeats as long as a condition stays true."
        print("\nQ3:", q3)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "T":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, because the statement is correct.")

        q4 = "Never stop a loop once it starts."
        print("\nQ4:", q4)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "F":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, use 'break' to stop a loop.")

        q5 = "Loops cannot be nested."
        print("\nQ5:", q5)
        while True:
            user = input("Enter Answer (T OR F) :").upper()
            if user == "T" or user == "F":
                break
            else:
                print("Enter T OR F ONLY!")
        if user == "F":
            print("CORRECT")
            score += 1
        else:
            print("WRONG ANSWER, nested loops are allowed, one loop inside another.")
    else:
        print("Invalid lesson number!")
        total_quiz = 0

    if total_quiz > 0:
        print(f"Total Score: {score}/{total_quiz}")

    if selected_count == 5:
        print("ALL 5 TOPICS COMPLETED!")
        break

print("Name:", name)
print("Student Number:", student_number)
print("Congrats, learn from it!")
