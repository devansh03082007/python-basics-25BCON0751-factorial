# README Claims Audit

Audit of the claims in `README.md` against the actual code in `factorial.py`.

| # | Claim | Verdict | Evidence from code |
|---|---|---|---|
| 1 | Calculates the factorial of a non-negative integer | Supported | `for i in range(2, n + 1): result *= i` |
| 2 | Prompts the user for a number | Supported | `input("Enter a number: ")` |
| 3 | Validates the input | Not Supported | Only negatives are checked (`if n < 0`). `int(input(...))` raises `ValueError` on `abc` or `3.5` |
| 4 | Prints the result | Supported | `print(f"{num}! = {factorial(num)}")` |
| 5 | `0! = 1` | Supported | `range(2, 1)` is empty, so `result` stays `1` |
| 6 | Iterative implementation | Supported | Uses a `for` loop, no recursion |
| 7 | No recursion depth limits | Supported | The function never calls itself |
| 8 | Handles negative input with a clear message | Supported | `return "Factorial not defined for negative numbers"` |
| 9 | Works with very large numbers | Supported | Python ints are unbounded (limited only by time and memory) |
| 10 | No external dependencies | Supported | No `import` statements |
| 11 | Requires Python 3.6+ | Supported | f-strings need Python 3.6+ |
| 12 | Can be imported with `from factorial import factorial` | Not Supported | No `if __name__ == "__main__":` guard, so importing runs `input()` and waits for the user |
| 13 | Example: `5` gives `5! = 120` | Supported | Loop result |
| 14 | Example: `0` gives `0! = 1` | Supported | Same as claim 5 |
| 15 | Example: `-3` gives `-3! = Factorial not defined for negative numbers` | Supported | Matches the f-string and the returned message |
| 16 | Project structure includes `README.md` and `LICENSE` | Unverified | Cannot be confirmed from the code |
| 17 | MIT License | Unverified | Not stated in the code |
| 18 | "Lightweight" and "beginner-friendly" | Unverified | Subjective, not checkable from code |

## Summary

- Not Supported: claims 3 and 12
- Unverified: claims 16, 17 and 18
- All other claims are Supported
