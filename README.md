# Are-you-smarter-than-a-5th-Grader-
Quiz based on are you smarter than a 5th grader show.


def check_guess(guess, answer):
    global score
    still_guessing = True
    attempt = 0
    while still_guessing and attempt < 3:
        if guess.lower() == answer.lower():
            print("Correct Answer")
            score += 1
            still_guessing = False
        else:
            if attempt < 2:
                guess = input("Wrong Answer, Try Again")
            attempt = attempt + 1
    if attempt == 3:
        print("The Correct answer is ",answer )
    
score = 0
print("Are you smarter than a 5th Grader? Made By: Theo Iatropoulos")
guess1 = input("So, Are you smarter than a 5th Grader?")
check_guess(guess1, "Yes")
guess2 = input("‌How many ‌days‌ ‌are‌ ‌there‌ ‌in‌ ‌a‌ ‌leap‌ ‌year?‌ ‌")
check_guess(guess2, "366")
guess3 = input( "How‌ ‌many‌ ‌days‌ ‌are‌ ‌there‌ ‌in‌ ‌July?‌ ‌")
check_guess(guess3, "31")
guess4 = input( " ‌What‌ ‌is‌ ‌88‌ ‌x‌ ‌10‌ ‌x‌ ‌0‌‌ ‌?‌ ‌")
check_guess(guess4, "0")
guess5 = input( " ‌Who was the first president? ‌")
check_guess(guess5, "George Washington")
guess6 = input("How many syllables are in the word Rhinoceros? Respond in a number")
check_guess(guess6, "4")
guess7 = input("How many continents are there?")
check_guess(guess7, "7")
guess8 = input("How much is 14 x 5")
check_guess(guess8, "70")
guess9 = input("What continent are the Pyramids of Giza located in?")
check_guess(guess9, "Africa")
guess10 = input("Which is the tallest mountain in the world?")
check_guess(guess10, "Mount Everest")
guess11 = input("Which is the thinnest layer of the Earth?")
check_guess(guess11, "Crust")
guess12 = input("Which‌ ‌is‌ ‌larger:‌ ‌10000 grams‌ ‌or‌ ‌one kilogram?‌ ‌")
check_guess(guess12, "10000 grams")

print("Congrats! Your Score is "+ str(score) ) 
