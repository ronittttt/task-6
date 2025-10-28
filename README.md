# task-6
This program creates 10 strong and complex passwords with random lengths between 16 and 32 characters.
Line-by-line explanation:


import secrets
Imports the secrets module, which is used to generate cryptographically secure random values.


import string
Imports the string module, which provides sets of characters like letters, digits, and punctuation.


import random
Imports the random module to randomly choose the password length.


for _ in range(10):
Loops 10 times to generate 10 different passwords.


length = random.randint(16, 32)
Chooses a random password length between 16 and 32 characters.


chars = string.ascii_uppercase + string.ascii_lowercase + string.digits + string.punctuation
Combines uppercase letters, lowercase letters, digits, and symbols into one character set.


print(''.join(secrets.choice(chars) for _ in range(length)))
Selects random characters from the combined set for the chosen length, joins them into a string, and prints the password.



Each password generated is unique, secure, and hard to guess — ideal for protecting sensitive accounts.
