# python-basics-25BCON0751-factorial
this is a python program to find factorial of any number 
# Factorial Calculator

A simple Python program that calculates the factorial of a non-negative integer.

## Description

This project provides a lightweight command-line tool for computing factorials. The `factorial.py` script prompts the user for a number, validates the input, and prints the result. It is a clean, beginner-friendly example of iterative problem solving in Python.

The factorial of a non-negative integer `n`, written `n!`, is the product of all positive integers less than or equal to `n`:

```
n! = n × (n - 1) × (n - 2) × ... × 2 × 1
```

By definition, `0! = 1`.

## Features

- Calculates the factorial of any non-negative integer
- Iterative implementation (no recursion depth limits)
- Handles negative input with a clear message
- Works with arbitrarily large numbers thanks to Python's big integers
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

When prompted, enter a non-negative integer and the program will print its factorial.

The function can also be imported into other Python code:

```python
from factorial import factorial

print(factorial(5))  # 120
```

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
└── LICENSE
```

## Contributing

Contributions, issues, and feature requests are welcome. Feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
