# Password-Suggestion-Tool-for-Web-Using-Python
A beginner-friendly project that generates strong, secure passwords for web applications. Features include customizable password length, a mix of uppercase and lowercase letters, numbers, and special characters. This tool ensures passwords meet common strength criteria and provides a simple command-line interface for user interaction.
Key Features:
1. Random password generation
2. Customizable length
3. Ensures strong password criteria
4. User-friendly command-line interface




import random
import string

val=string.ascii_letters+string.digits+string.punctuation


#using normal loop
list=""
for el in range(12):
  list+=random.choice(val)

print("your random password is=",list)


#using list comprihension
res="".join([random.choice(val) for i in range(12)])

print(res)
