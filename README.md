# Generating-random-password
Generating random password  using random module

## importing random module
import random
## giving length of password from the user
length_password = int(input("Enter the length of the password :"))
## Giving all alphabets in upper case format in s1 variable
s1 = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
## converting upper case letters into lower case letter using the lower function and store in s2 variable
s2 = s1.lower()
## all numbers from 0-9 and which are stored in s3 variable
s3 = "1234567890"
## all special type of characters in s4 variable
s4 = "!@#$%^&*()+/<>:{}[]"
## adding all variables into a s variable
s = s1+ s2+ s3+ s4
## using the random module selecting or generating the passworrd from s varible upto lengthof password
temp = random.sample(s, length_password)
a = "".join(temp)
## printing the password
print(f"Your password is {a}")
