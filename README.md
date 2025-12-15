# random password
import random
import string

def generate_password(length=12):
    letters = string.ascii_letters      # a-z A-Z
    digits = string.digits              # 0-9
    symbols = string.punctuation        # !@#$%^&* etc

    all_chars = letters + digits + symbols

    password = ''.join(random.choice(all_chars) for _ in range(length))
    return password

# User se length lena
length = int(input("Password ki length batao: "))
print("Generated Password:", generate_password(length))

