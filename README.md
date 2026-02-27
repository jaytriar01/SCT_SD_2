import random

def guess_the_number():
    # Generate a random number between 1 and 100
    secret_number = random.randint(1, 100)
    
    while True:
        # Prompt the user to input their guess
        user_guess = int(input("Enter your guess (1-100): "))
        
        # Compare the user's guess to the generated number
        if user_guess < secret_number:
            print("Too low! Try again.")
        elif user_guess > secret_number:
            print("Too high! Try again.")
        else:
            print("Congratulations! You guessed the number.")
            break

if __name__ == "__main__":
    guess_the_number()
