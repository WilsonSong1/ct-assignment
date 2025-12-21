# Computational Theory Assessment

# SHA-256 Implementation and Password Cracking Project

## Overview

This project implements the **SHA-256 cryptographic hash function** from first
principles and demonstrates its use in a **password cracking scenario**.
The work is structured as a series of problems that progressively build the
algorithm, starting from low-level bitwise operations and ending with a
dictionary attack on password hashes.

The project is intended for **educational purposes**, illustrating both how
SHA-256 works internally and why insecure password hashing practices are
vulnerable to attack.

---

## Project Contents

The project consists of the following files:

- `problems.ipynb` — Main Jupyter Notebook containing all implementations and explanations  
- `requirements.txt` — Python dependencies required to run the notebook  
- `100k-most-used-passwords-NCSC.txt` — Password wordlist used in Problem 5  

---

## Problem Breakdown

### Problem 1 — Binary Words and Operations
Implements the core bitwise functions required by SHA-256, including Parity,
Choose (Ch), Majority (Maj), bit rotations, shifts, and sigma functions.

### Problem 2 — Fractional Parts of Cube Roots
Generates SHA-256 round constants using the fractional parts of cube roots of
prime numbers, following the NIST specification.

### Problem 3 — Padding
Implements SHA-256 message padding and splits messages into 512-bit blocks.

### Problem 4 — Hashes
Combines all previous components into a complete SHA-256 hash implementation.

### Problem 5 — Passwords
Demonstrates a **dictionary attack** against unsalted SHA-256 password hashes
using a list of commonly used passwords.

---
## Environment Setup

This project was developed on **Python 3.11.9**.

From the project directory, open a terminal and set up the environment by creating and activating a virtual environment, then installing the required dependencies:

```bash
python3 --version
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```