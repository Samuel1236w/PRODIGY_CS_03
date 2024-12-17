import re

def password_complexity_checker(password):
    """
    Function to assess the strength of a given password
    based on length, use of uppercase, lowercase, digits, and special characters.

    Parameters:
    - password (str): The password to check

    Returns:
    - strength (str): Feedback on the password strength
    """

    # Initialize criteria checks
    length_criteria = len(password) >= 8  # Password should be at least 8 characters long
    uppercase_criteria = bool(re.search(r'[A-Z]', password))  # Should contain at least one uppercase letter
    lowercase_criteria = bool(re.search(r'[a-z]', password))  # Should contain at least one lowercase letter
    digit_criteria = bool(re.search(r'\d', password))  # Should contain at least one numeric digit
    special_char_criteria = bool(re.search(r'[!@#$%^&*(),.?":{}|<>]', password))  # Should contain a special character

    # Calculate the total number of criteria met
    criteria_met = sum([length_criteria, uppercase_criteria, lowercase_criteria, digit_criteria, special_char_criteria])

    # Provide feedback based on the number of criteria met
    if criteria_met == 5:
        return "Strong Password: Your password meets all the recommended criteria."
    elif criteria_met == 4:
        return "Moderate Password: Your password is good, but consider adding more complexity."
    elif criteria_met == 3:
        return "Weak Password: Your password is weak. Add more complexity to secure it."
    else:
        return "Very Weak Password: Your password is too simple. Make it longer and include a mix of characters."

# Main program to interact with the user
def main():
    """
    Main function to get user input and evaluate password strength.
    """
    print("Welcome to the Password Complexity Checker!")
    password = input("Enter your password to check its strength: ")
    feedback = password_complexity_checker(password)
    print("\nPassword Strength Assessment:")
    print(feedback)

# Execute the main program when the script is run
if __name__ == "__main__":
    main()
