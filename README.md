# Prompt the user to enter a single char

char_input = input("Enter a single character: ")

# Check if the input is exactly 1 character and if it is a letter

if len(char_input) == 1 and char_input.isalpha():
    char = char_input.lower()

    # Check if the char is a vowel
    if char in "aeiou":
        print("The character is a vowel")

    else:
        print("The character is a consonant")
else:
    if len(char_input) != 1:
        print("Error: Please enter only one character")
    else:
        print("Error: The input is not a letter")
