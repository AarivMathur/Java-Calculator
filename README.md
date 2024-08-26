# Calculator Project - README

## Project Overview

This project contains two main classes: `Calculator` and `CalculatorTester`. The `Calculator` class provides basic arithmetic methods to perform operations like addition and multiplication. The `CalculatorTester` class is designed to test these methods and demonstrate how they work.

### Classes:
1. **Calculator**
   - This class provides methods for performing basic arithmetic operations (sum and multiplication).
   - It has no instance variables or constructor, so you can instantiate it using empty parentheses: `Calculator c = new Calculator();`.

2. **CalculatorTester**
   - This class contains the `main` method, which creates a `Calculator` object and calls its methods to demonstrate functionality.

## Class: `Calculator`

### Methods:

1. **`sum(int x, int y)`**:
   - This method prints the sum of two integers, `x` and `y`.
   - Example:
     ```java
     calc.sum(3, 10);
     // Output: 3 + 10 = 13
     ```

2. **`multiply(int x, int y)`**:
   - This method prints the product of two integers, `x` and `y`.
   - Example:
     ```java
     calc.multiply(-5, -7);
     // Output: -5 * -7 = 35
     ```

## Class: `CalculatorTester`

This class contains the main method and tests the `Calculator` class.

### `main(String[] args)`:
- Creates a `Calculator` object: `Calculator calc = new Calculator();`
- Demonstrates the `sum` and `multiply` methods:
    ```java
    calc.sum(3, 10);          // Outputs: 3 + 10 = 13
    calc.multiply(-5, -7);    // Outputs: -5 * -7 = 35
    ```

- The program also shows that changes to variables inside methods do not affect the original variable unless explicitly changed in the calling class:
    ```java
    int x = 5;
    calc.addFive(x);          // This method call will not affect the value of `x` in this scope
    System.out.println(x);    // Outputs: 5
    ```

## How to Run

1. Compile both the `Calculator` and `CalculatorTester` classes.
2. Run the `CalculatorTester` class, which will call the `sum` and `multiply` methods and display their results.
