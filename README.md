# project_One
#Team Project 1#
# ITS 250- Programming I- Fall 2021 Project # 1
## Variables, Constants, Operators (logical, arithmetical, assignment),
## Conditional Operator, While Loops, Reading input, Performing Calculations,
## If Statements, If-else Statements, For Loops, and Functions

# Factors of Military Enlistment and Disqualifiers
## "Creating a program discriminating the factors of military enlistment. Using the lectured information on loops, constants, 
##  variable attributions we will develop a program that upon completion of the questionnaire will determine whether or not 
## an individual is or is not eligible for enlistment." 
age = 100
ASVAB_score = 99
good_credit = 650
bad_credit = 649

print("Please fill out questionnaire truthfully")
l = ["Thank you for your honesty"]
for i in l:
    print(i)

## This part of the program defines the basic info starting##
## the program##
def main():
    first_name = input('Enter your first name: ')
    last_name = input('Enter your last name: ')
    current_education = input('Enter your Ed: ')
    height = input('Enter your height in inches: ')
    weight = input('Enter your weight: ')
    disqualifiers ()

## This disqualifier descriminates for the
## over the age limit
## for the military
def disqualifiers():
    age = int(input('Enter your age: ')) 
    if age <= 42:
        print (' Qualified for age ')
    elif age > 42:
        print ('Disqualified for age')
    disqualifiers2()

## This disqualifier decriminates the passing ASVAB score
def disqualifiers2():
    ASVAB_score = int(input('Enter ASVAB score:'))
    if ASVAB_score >= 31:
        print ('Qualified for score')
    elif ASVAB_score < 31:
        print ('Disqualified for score ')
    disqualifier3()
    
## This disqualifier desciminates Credit acceptance for the military##
def disqualifier3():
    credit_score = int(input("Enter your Credit Score:"))
    while bad_credit >= 649:
        if credit_score >= good_credit:
            print('Your Credit Score is good')
        else: 
            print('Your Credit Score is Bad')
        break
        
main ()
