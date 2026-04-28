# arithmetic-formatter-project
This project contains a function called arithmetic_arranger that formats a list of arithmetic problems vertically and side-by-side, similar to how they are written on paper.

## Features
- Accepts up to 5 arithmetic problems
- Supports addition(+) and subtraction(-)
- Properly aligns numbers for readability
- Optionally displays the answers
- Includes input validation with clear error messages

 ## How It Works 
 1. Check the number of problems
    - If there are more than 5 problems, return an error message.
 2. Loop through each problem
    - Split into:
        - First number(num1)
        - Operatr(+ or -)
        - Second number(num2)
  3. Validation check
     - Operator must be + or -.
     - Numbers can only contain digits.
     - Numbers can have at most 4 digits. 
  4. Formatting
     - Determine the width using width = max(len(num1), len(num2)) + 2
     - Right-align numbers using .rjust()
     - Build:
         - top row
         - bottom row
         - dash row
  5. Optional Answer Calculation
     - Execute the code using eval(f"{num1} {operator} {num2}
  6. Combine rows
      - Join problems with 4 spaces
      - Return formatted string
  
