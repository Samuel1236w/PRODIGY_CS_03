OVERVIEW

The Password Complexity Checker helps users ensure their passwords meet recommended security guidelines. It categorizes passwords as:
     
 - Strong: Meets all complexity requirements. 
 - Moderate: Meets most but not all criteria.
 - Weak: Needs significant improvement.
 - Very Weak: Highly insecure.

   FEATURES

   Checks if a password has:
- Minimum length of 8 characters
- At least one uppercase letter
- At least one lowercase letter
- At least one digit
- At least one special character

  HOW IT WORKS

The script evaluates the password using regular expressions:

a. It checks the password for specific patterns (uppercase, lowercase, digits, special characters).

b. Based on the number of criteria met, it classifies the password into one of four categories:
  - Strong
  - Moderate
  - Weak
  - Very Weak

REQUIREMENTS

  - Python 3.x
  - No external libraries required

HOW TO RUN

1. Clone the Repository

git clone https://github.com/yourusername/password-complexity-checker.git
cd password-complexity-checker


2. Run the Script
Ensure Python is installed on your system, then execute:

    - python password_checker.py

3. Input Your Password
Follow the prompts to check your password’s strength




