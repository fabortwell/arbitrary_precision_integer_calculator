# Arbitrary Precision Integer Calculator

This project implements an **arbitrary-precision integer calculator** in Python, without relying on native support for big integers or external libraries for core functionality. It handles mathematical operations on very large integers by using strings for number representation and basic algorithms for arithmetic operations.

## Features

- **Supported Operations:**
  - **Addition**: e.g., `1678912653456789 + 987651257924321`
  - **Subtraction**: e.g., `987623111348821987654321 - 1236535787223456789`
  - **Multiplication**: e.g., `123456789 * 987654321`
  - **Division** (with remainder): e.g., `987654321 / 123456789`
  - **Factorial**: e.g., `100!`
- **Handles Very Large Numbers**: Works with numbers far exceeding native integer limits.
- **REPL Interface**: A simple interactive shell for entering expressions.

## How It Works

The calculator uses strings to represent numbers and implements algorithms for arithmetic operations:
- **Addition and Subtraction**: Operate digit by digit, managing carry and borrow.
- **Multiplication**: Simulates long multiplication.
- **Division**: Uses repeated subtraction to compute the quotient and remainder.
- **Factorial**: Iteratively multiplies numbers from 1 to the input value.

### Limitations
- Does not support decimal (floating-point) numbers.
- Only operates on integers (no fractions, non-decimal bases, or advanced functions like logarithms).
- Limited error handling for complex expressions.

## Installation

1. Clone the repository:
   ```bash
   git clone git@github.com:fabortwell/arbitrary_precision_integer_calculator.git
   ```
2. Navigate to the project directory:
   ```bash
   cd arbitrary-precision-calculator
   ```
3. Run the calculator script:
   ```bash
   python calculator.py
   ```

## Usage

1. Launch the program. You’ll enter a **Read-Eval-Print Loop (REPL)** interface.
2. Type a mathematical expression, e.g.:
   ```plaintext
   > 123456789 + 987654321
   1111111110
   ```
3. Supported operations:
   - Addition: `123 + 456`
   - Subtraction: `987 - 654`
   - Multiplication: `123 * 456`
   - Division: `987 / 123`
     - Returns both **quotient** and **remainder**.
   - Factorial: `100!`
4. Type `exit` to quit.

### Example Session

```plaintext
> 150!
57133839564458545904789328652610540031895535786011264182548375833179829124845398393126574488675311145377107878746854204162666250198684504466355949195922066574942592095735778929325357290444962472405416790722118445437122269675520000000000000000000000000000000000000
> 272738849282737282 + 21819291901919
272760668574639201
> 
```

## Code Structure

![image](https://github.com/user-attachments/assets/11733a4d-fbc4-4af5-a3e9-337c30410d1d)

- **REPL**: Provides an interactive shell for user input and result display.

## Contributing

Feel free to submit issues or pull requests. Suggestions for extending functionality (e.g., fractions, logarithms, or non-decimal bases) are welcome!

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---
