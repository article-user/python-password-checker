# Password Checker
# Beginner Python project
# Checks if a password is strong based on length, number, and uppercase letter

print("Welcome to Password Checker")

# Take password input from user
password = input("Enter your password: ")

# Initialize flags
has_number = False
has_upper = False

# Check each character in the password
for char in password:
    if char.isdigit():
        has_number = True
    if char.isupper():
        has_upper = True

# Check all conditions
if len(password) >= 8 and has_number and has_upper:
    print("✅ Strong password")
else:
    print("❌ Weak password")
    print("Password must:")
    print("- be at least 8 characters")
    print("- contain a number")
    print("- contain an uppercase letter")
