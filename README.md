# Python Substitution Cipher

## Project Description
This is a simple Python encryption and decryption program that uses a **Substitution Cipher** technique.

The program replaces each character in the original message (plaintext) with another randomly shuffled character to produce an encrypted message (ciphertext).

It can also decrypt the encrypted message back into its original form using the same encryption key.

## Technologies Used
- Python 3
- `random` module
- `string` module

## Features
- Generates a collection of letters, numbers, and punctuation marks.
- Randomly shuffles characters to create an encryption key.
- Encrypts user-provided messages.
- Decrypts encrypted messages.
- Uses character indexing to match original and replacement characters.

## How It Works

### 1. Character Generation
The program combines:
- `string.punctuation` – special characters.
- `string.digits` – numbers (0–9).
- `string.ascii_letters` – uppercase and lowercase letters.

### 2. Key Generation
The original character list is copied using `.copy()` and shuffled using `random.shuffle()`.

### 3. Encryption
The program:
1. Takes a message from the user.
2. Finds each character's index in the original list.
3. Uses that index to find its replacement in the shuffled key.
4. Builds the encrypted message.

### 4. Decryption
The program:
1. Takes an encrypted message.
2. Finds each character's index in the shuffled key.
3. Uses that index to retrieve the original character.
4. Reconstructs the original message.

## How to Run

1. Make sure Python 3 is installed.
2. Copy the Python code into a file named `main.py`.
3. Open a terminal in the project directory.
4. Run:

```bash
python main.py
```

5. Enter a message to encrypt.
6. Enter the encrypted message when prompted for decryption.

## Python Concepts Practiced
- Importing modules
- Variables and data types
- Strings and lists
- User input with `input()`
- For loops
- Conditional statements
- List indexing
- String concatenation
- List copying
- Random shuffling
- Encryption and decryption logic

## Limitations
- The encryption key is randomly generated every time the program runs.
- The same key must be used for successful decryption.
- The program is for educational purposes and is not suitable for securing sensitive information.
- The encryption method is not considered secure by modern cryptographic standards.

## Learning Objective
The objective of this project is to understand the basic principles of encryption and decryption while practising Python programming concepts and learning how substitution ciphers work.

## Author
Created as a Python learning project. Dave Odoung

---

**Note:** This project demonstrates a basic substitution cipher for educational purposes only.
