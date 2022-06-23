# My First Python String


name = input("What is your name? ")
print("Hello " + name)
age = input("thank you for that information, how old are you? ")

-------------------------------------------------------------------------------
-above is my first attempt at creating a system used to gather customer information. at this point its extremely simple but i believe i can make it better on line 3 
to be more accurate in gaining an age. but also after some research sometimes simple is better however id like to practice so im going to move forward with a different line on line 3
--------------------------------------------------------------------------------

name = input("What is your name? ")
print("Hello " + name)
birth_year = input("thank you, could you please enter your birth year? ")
age = (2022 - birth_year)
print(age)

-----------------------------------------------------------------------------------

-now i have attempted to have the computer calculate the age based off the users birth year. unfortunately at line 12-13 instead of printing the desired "age" 
such as in my case it should say "22" im getting an error "Traceback (most recent call last):
  File "c:\terraform\demo\first project.py\firstfile.py", line 4, in <module>
    age = (2022 - birth_year)
TypeError: unsupported operand type(s) for -: 'int' and 'str'"
so im looking aat rewriting that line slightly different in an attempt to fix that. maybe defining age in a different line than im using to do the math calculating it?
after some research online it seems i was wrong. the error was because i tried to subtract a string from intenger which essentially means im trying to subtract one value
from another that arent compatible. literally comparing apples to oranges. somehow i need to convert the value so i will take time as im writing this to do so. in this
case it appears id need to use "int(birth_year)" to replace the "birth_year" in the code. lets try that and see how it works.
  
  
-----------------------------------------------------------------------------------------

code as written now:

name = input("What is your name? ")
print("Hello " + name)
birth_year = input("thank you, could you please enter your birth year? ")
age = 2022 - int(birth_year)
print(age)

----------------------------------------------------------------------------------
  
  
it appears to have worked! now when i put in my name/ birthyear it will retain that information. now i think id like to refine the birthdate from more than a year toa birth month as well.
i believe it would help the accuracy of the information as i am 21 and turning 22 next month however that code would print im 22 not 21 as its calculating only based off years.
i will revise at a later date. for now this is my first independant python code!
  
  
-----------------------------------------------------------------------------------


exampple of how it worked:

What is your name? (i typed "ryan")
Hello ryan
thank you, could you please enter your birth year? (i typed "2000")
22


base:
What is your name? ryan
Hello ryan
thank you, could you please enter your birth year? 2000
22
  
  
---------------------------------------------------------------------------------------
