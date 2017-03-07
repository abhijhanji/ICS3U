#Strand 1 Summative 
#Name: Abhi Jhanji
#March 2, 2016
#Purpose: This programs purpose is to list the Digits of an input number and sum those numbers
#----------------------------------------------------------------------------------------------

#Here I am importing libraries I may need to use in the program, Math lib, and easygui

from math import*
from easygui import*

#This section will obtain the input from the user
#asking if the user would like to use program to determine digits and sum of digits of a number
choices = ["yes","no"]
use_program = buttonbox("would you like to find the amount of digits in your number, and the sum of those digits?", choices = choices)
if use_program == "no":
  exit()


#Using a button box to filter the choices by the user
choices = ["2 digit number","3 digit number","4 digit number"]
your_number = buttonbox("How long is your number?", choices = choices)

#Going through the procedure for the first choice "2 digit"

if your_number == "2 digit number":
    #entering the number
    number = enterbox("Please enter your number")
    #Promtpting the user to enter a number only 2 digits long if they enter one greater or less than that
    if len(number) >2 or  len(number) <2:
        number = enterbox("Please enter a number that is two digits")
    #returning to the original if statement
    digit_1 = str(number)[0] #setting the first digit equal to digit 1
    digit_2 = str(number)[1] #setting the second digit equal to digit 2
    sum_of_digits = int(digit_1) + int(digit_2) #setting sum of the digit to the sum od the digits
    #displaying the digits and sum
    msgbox("your first digit is " + digit_1 + "\n your second digit is " + digit_2 +"\n the sum of your digits is " + str(sum_of_digits))



if your_number == "3 digit number":
    #entering the number
    number = enterbox("Please enter your number")
    #Promtpting the user to enter a number only 2 digits long if they enter one greater or less than that
    if len(number) >3 or  len(number) <3:
        number = enterbox("Please enter a number that is two digits")
    #returning to the original if statement
    digit_1 = str(number)[0] #setting the first digit equal to digit 1
    digit_2 = str(number)[1] #setting the second digit equal to digit 2
    digit_3 = str(number)[2] #setting the second digit equal to digit 3
    sum_of_digits = int(digit_1) + int(digit_2) + int(digit_3) #setting sum of the digit to the sum of the digits
    #displaying the digits and sum
    msgbox("your first digit is " + digit_1 +"\n your second digit is " + digit_2 +"\n your third digit is " + digit_3 + "\n the sum of your digits is" + str(sum_of_digits))



if your_number == "4 digit number":
    #entering the number
    number = enterbox("Please enter your number")

    #Promtpting the user to enter a numbe ronly 2 digits long if they enter one greater or less than that
    if len(number) >4 or  len(number) <4:
        number = enterbox("Please enter a number that is 4 digits")

    #returning to the original if statement
    digit_1 = str(number)[0] #setting the first digit equal to digit 1
    digit_2 = str(number)[1] #setting the second digit equal to digit 2
    digit_3 = str(number)[2] #setting the third digit equal to digit 3
    digit_4 = str(number)[3] #setting the fourth digit equal to digit 4
    sum_of_digits = int(digit_1) + int(digit_2) + int(digit_3) + int(digit_4) #setting sum of the digit to the sum of the digits
    #displaying the digits and sum
    msgbox("your first digit is " + digit_1 + "\n your second digit is " + digit_2 + "\n your third digit is " + digit_3 + "\n your fourth digit is " + digit_4 +  "\n the sum of your two digits is "   + str(sum_of_digits))
