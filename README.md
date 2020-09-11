# you only have three chances!
from random import seed
from random import randint
print('guess a number between 1 to 10')
secret_number = randint(0,10)
guess_limit = 3
guess_count = 0
while guess_count < guess_limit:
    guess = int(input('guess: '))
    guess_count = guess_count + 1
    if guess == secret_number:
        print('you have won!!')
        break
else:
    print('you have failed!')
