# Task-3
"""A password generator is a useful tool that generates strong and  random passwords for users. This project aims to create a password generator application using Python, allowing users to  specify the length and complexity of the password."""
import random
import string

def generate_password(length):
    characters = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(random.choice(characters) for _ in range(length))
    return password

length = int(input("Enter password length: "))
print("Generated Password:", generate_password(length))
