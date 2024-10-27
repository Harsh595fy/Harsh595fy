import re

def check_password_strength(password):
    criteria = {
        "length": len(password) >= 8,
        "uppercase": bool(re.search(r'[A-Z]', password)),
        "lowercase": bool(re.search(r'[a-z]', password)),
        "digits": bool(re.search(r'[0-9]', password)),
        "special_chars": bool(re.search(r'[!@#$%^&*()_+=]', password))
    }
    strength = sum(criteria.values())
    if strength == 5:
        return "Strong"
    elif 3 <= strength < 5:
        return "Moderate"
    else:
        return "Weak"

password = input("Enter your password: ")
print("Password Strength:", check_password_strength(password))
