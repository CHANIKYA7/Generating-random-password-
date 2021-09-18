# Generating-random-password-
Generating random password  using random module


import random
length_password = int(input("Enter the length of the password :"))
s1 = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
s2 = s1.lower()
s3 = "1234567890"
s4 = "!@#$%^&*()+/<>:{}[]"
s = s1+ s2+ s3+ s4
temp = random.sample(s, length_password)
a = "".join(temp)
print(f"Your password is {a}")
