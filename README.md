# python
import random
def main():
secret = random.randint(1, 100)
attempts = 0
print("Guess the number (1-100)!")
guess = 0
while guess != secret:
guess = int(input("Enter your guess: "))
attempts += 1
if guess > secret:
print("Too high!")
elif guess < secret:
print("Too low!")
else:
print(f"Correct! Attempts: {attempts}")
main()