# 🔐 Password Strength Checker

A beginner-friendly Python program that checks how strong a password is and tells you exactly what is missing.

## ✨ Features
- Checks for lowercase letters (a-z)
- Checks for uppercase letters (A-Z)
- Checks for numbers (0-9)
- Checks for symbols (! @ # $ % ...)
- Checks for a minimum length of 8 characters
- Gives clear tips to improve a weak password
- Runs in a loop until you type `q`

## 🛠️ Requirements
- Python 3.x
- No extra libraries needed (uses only the built-in `string` module)

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/prashantgautamdev/password-strength-checker.git
   ```
2. Go into the folder:
   ```bash
   cd password-strength-checker
   ```
3. Run the program:
   ```bash
   python password_strength_checker.py
   ```

## 📸 Example

```
Enter password (or 'q' to quit): hello
Not a strong password
 - Use at least 8 characters
 - Add an uppercase letter
 - Add a number
 - Add a symbol like @, #, !

Enter password (or 'q' to quit): Hello@123
Strong password
```

## 🧠 How It Works
The program uses `any()` with a generator to check each character of the password:

```python
has_digit = any(c.isdigit() for c in passwd)
```

A password is "Strong" only if it has all four character types and is at least 8 characters long.

## 📚 What I Learned
- How `any()` works with a generator expression
- The difference between `isalpha()`, `isdigit()`, `isupper()` and `islower()`
- Using `string.punctuation` from the built-in `string` module
- Debugging typos and common errors (`NameError`, `TypeError`)
- Using `while True` loops with `break`

## 🔮 Future Improvements
- Add a strength score (weak / medium / strong)
- Hide the password while typing using `getpass`
- Check against a list of common passwords
- Build a simple GUI

## 👤 Author
**Your Name**
- GitHub: [prashantgautamdev](https://github.com/prashantgautamdev)
- LinkedIn: [Prashant Gautam](https://www.linkedin.com/in/prashantcode/)

## 📄 License
This project is open source and free to use for learning.
