# Python
#Write function to creat password random by python
import random
import string

def generate_password(length):
    # Define the characters that can be used in the password
    charset = string.ascii_letters + string.digits + string.punctuation

    # Generate the password
    password = ''.join(random.choice(charset) for _ in range(length))

    return password

# Usage example
password_length = int(input("Enter the length of the password: "))
password = generate_password(password_length)
print("Generated Password:", password)
