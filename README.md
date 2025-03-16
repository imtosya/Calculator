# Calculator
This is a console-based calculator program written in Java that performs basic arithmetic operations and supports advanced mathematical functions. The program allows users to input expressions for addition, subtraction, multiplication, division, modulus, as well as functions like absolute value, square root, power, and rounding. Additionally, it features a history function to display past calculations and provides error handling for invalid input.

**Features**:  
- **Basic Arithmetic Operations**: Supports addition (`+`), subtraction (`-`), multiplication (`*`), division (`/`), and modulus (`%`).  
- **Advanced Functions**:  
  - `abs(number)`: Returns the absolute value of the number.  
  - `sqrt(number)`: Returns the square root of the number.  
  - `pow(base, exponent)`: Raises `base` to the power of `exponent`.  
  - `round(number)`: Rounds the number to the nearest integer.  
- **History Feature**: Stores and displays past calculations.  
- **Error Handling**: Catches invalid input and handles division by zero errors.  
- **Exit Option**: Users can exit the program by typing `exit`.

**How to Use**:  
1. Start the program, and you will be prompted to enter an arithmetic expression.  
2. Enter your desired expression, which can include operators (`+`, `-`, `*`, `/`, `%`) and functions like `abs()`, `sqrt()`, `pow()`, and `round()`.  
3. The result of the calculation is displayed after the input is processed.  
4. To view past calculations, type `history`.  
5. After each calculation, the program will ask if you want to continue or exit the program. Type `y` to continue or `n` to exit.

**Example Inputs and Outputs**:  
1. **Input**: `abs(-10) + sqrt(25) * 3`  
   **Output**: `Result: 25.0`

2. **Input**: `pow(2, 3) + 10`  
   **Output**: `Result: 18.0`

3. **Input**: `history`  
   **Output**: Shows a list of past calculations.

**Functions in Detail**:  
- **Basic Operations**: The program follows standard mathematical precedence rules for operators. For example, multiplication (`*`) and division (`/`) have higher precedence than addition (`+`) and subtraction (`-`).  
- **Function Processing**: Functions like `abs()`, `sqrt()`, `pow()`, and `round()` are processed before basic operations in the expression. The program extracts the function's arguments, performs the operation, and replaces the function in the expression with the result.

**Error Handling**:  
- The program checks for invalid expressions and will display an error message like "Invalid expression! Please check the format."  
- If there is an attempt to divide by zero, it prints an error message: "Error: Division by zero!"

**Structure**:  
- **Stacks**: The program uses two stacks: one for operators and one for operands. As the program parses the expression, it pushes operators onto the operator stack and operands onto the operand stack. Once the entire expression is processed, it pops the stacks to perform calculations based on mathematical precedence.  
- **History**: After each calculation, the program stores the result in a history list, allowing users to recall previous calculations.

**Conclusion**:  
This calculator program is a useful tool for performing both basic and advanced arithmetic calculations. It provides users with a history of past calculations and handles errors gracefully. The program allows continuous operation without needing to restart, making it a convenient and efficient tool for everyday use.
