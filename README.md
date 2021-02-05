# This is a Python Project #1 Random Password Generator (RPG)

#This is a program that i made in python to generate a random password

#Starting:

from random import randint

lower = "abcdefghijklmnopqrstuvwxyz"
upper = lower.upper()
numbers = "1234567890"
special_characters = "!@#$%^&*()+:?\|"

password_stuff = lower + upper + numbers + special_characters

password_length = int(input("Enter the length of Password : "))
password = ""
length = 0

if password_length < 8 :
    print("Password length must be up to 8 Characters")

else :
    while length<password_length:
        password = password + password_stuff[randint(0,len(password_stuff)-1)]
        length += 1
    print("Generated Password :",password )

#end.
