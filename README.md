# TCS-332
It is our project for Fundamentals of information security and blockchain (TCS 332)

 🔐 Smart Password Strength Analyzer and Crack Time Estimator

## 📌 About the Project

The *Smart Password Strength Analyzer and Crack Time Estimator* is a Python-based cybersecurity project that analyzes password strength and estimates the time required to guess a password under different attack assumptions.

The program checks password length, uppercase and lowercase letters, numbers, and special characters. It calculates a security score, estimates password entropy, predicts cracking time for online and offline attacks, and provides suggestions to improve password security.

This project aims to promote cybersecurity awareness and demonstrate fundamental password security concepts.

## 🎯 Objectives

- Analyze password strength using basic security rules.
- Check password length and character diversity.
- Identify selected commonly used passwords.
- Calculate estimated password entropy.
- Estimate password-cracking time for online and offline attacks.
- Provide recommendations for improving password security.

## ✨ Features

- *Password Strength Analysis:* Checks password length and character types.
- *Security Score:* Assigns points based on five password criteria.
- *Common Password Detection:* Checks against a predefined list of common passwords.
- *Entropy Calculation:* Estimates password entropy in bits.
- *Crack Time Estimation:* Calculates estimated guessing time for online and offline attacks.
- *Automatic Time Conversion:* Displays estimated time in seconds, minutes, hours, days, or years.
- *Security Recommendations:* Suggests improvements when password criteria are not satisfied.
- *Command-Line Interface:* Displays results directly in the terminal.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| re   | Checks password character patterns using regular expressions |
| math | Calculates logarithms and powers |
|string| Provides the set of punctuation characters |

## ⚙️ How the Project Works

1. *Password Input:* The user enters a password.
2. *Strength Analysis:* The program checks length, uppercase letters, lowercase letters, digits, and special characters.
3. *Common Password Check:* The entered password is compared with a predefined list of common passwords.
4. *Entropy Calculation:* The program estimates the character-set size and calculates entropy.
5. *Crack Time Estimation:* It estimates the guessing time using assumed online and offline guessing speeds.
6. *Result Display:* The program displays the strength category, security score, entropy, estimated crack times, and recommendations.

## 📊 Password Strength Classification

The program assigns a score based on five criteria.

| Score | Classification |
|---|---|
| 0–2 | Weak |
| 3–4 | Medium |
| 5   | Strong |

*Note:* The current code produces three categories: Weak, Medium, and Strong.

## 🧮 Entropy and Crack Time

The program estimates entropy using the formula:

[ H=L\log_2(R) ]

Where:

- H = estimated entropy in bits
- L = password length
- R = estimated size of the character set

It then estimates the number of possible combinations:

[ N=2^H ]

The program uses these assumed guessing speeds:

- Online attack: 100 guesses per second
- Offline attack: 100,000 guesses per second

The estimated time is calculated using half the search space on average.

*Important:* These are simplified estimates, not guarantees of real-world cracking time. Actual results depend on password patterns, attacker capabilities, hardware, rate limits, and the password-hashing method.

  Security and Limitations

- The program uses basic password rules and a small predefined list of common passwords.
- It does not use an external password-strength library or a real password-cracking engine.
- Entropy and crack-time results are theoretical estimates and may not reflect actual attack conditions.
- Use test passwords rather than real account passwords when demonstrating the project.
- Password strength also depends on unpredictability and whether the password has been reused or exposed.

 Future Scope

- Add a graphical user interface using Tkinter.
- Improve common-password and predictable-pattern detection.
- Integrate a random password generator to generate strong and unique passwords using uppercase letters, lowercase letters, numbers, and special characters.
- Improve crack-time estimation using configurable attack assumptions.
- Add an option to export password security reports.

 Learning Outcomes

This project provides practical experience with Python programming, regular expressions, mathematical calculations, conditional statements, lists, loops, and functions. It also introduces password entropy, brute-force guessing, and basic cybersecurity practices.

 Project Contributors

- Gaurav Singh Negi
- Gagandeep Kaur

## 🏷️ Project Information

- *Project:* Smart Password Strength Analyzer and Crack Time Estimator
- *Domain:* Cybersecurity
- *Language:* Python

---

Built to explore password security and promote better cybersecurity awareness.
