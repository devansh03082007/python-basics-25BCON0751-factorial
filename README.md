# python-basics-25BCON0751-factorial
this is a python program to find factorial of any number 
# Factorial Calculator

A Python program that calculates the factorial of a non-negative integer.

## Description

`factorial.py` prompts the user for a number and prints its factorial.

The factorial of a non-negative integer `n`, written `n!`, is the product of all positive integers less than or equal to `n`:

```
n! = n × (n - 1) × (n - 2) × ... × 2 × 1
```

By definition, `0! = 1`.

## Features

- Calculates the factorial of a non-negative integer
- Iterative implementation (no recursion depth limits)
- Shows a message for negative input
- Supports very large results using Python's built-in big integers
- No external dependencies

## Requirements

- Python 3.6 or higher

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   ```

2. Navigate to the project directory:

   ```bash
   cd <your-repo-name>
   ```

No additional packages need to be installed.

## Usage

Run the script from your terminal:

```bash
python factorial.py
```

Enter a whole number when prompted. The program prints its factorial.

## Example

```
$ python factorial.py
Enter a number: 5
5! = 120
```

```
$ python factorial.py
Enter a number: 0
0! = 1
```

```
$ python factorial.py
Enter a number: -3
-3! = Factorial not defined for negative numbers
```

## Project Structure

```
.
├── factorial.py
├── README.md
└── audit.md
```
