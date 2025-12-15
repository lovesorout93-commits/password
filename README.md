# random password
import random

print("🎲 Welcome to Number Guessing Game")
print("Main 1 se 100 ke beech ek number soch raha hoon...")

number = random.randint(1, 100)
attempts = 0

while True:
    guess = int(input("Apna guess daalo: "))
    attempts += 1

    if guess < number:
        print("📉 Too Low! Dobara try karo.")
    elif guess > number:
        print("📈 Too High! Dobara try karo.")
    else:
        print(f"🎉 Mubarak ho! Tumne {attempts} attempts me sahi guess kar liya.")
        break
