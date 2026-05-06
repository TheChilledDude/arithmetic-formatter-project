# arithmetic-formatter-project
This project contains a Python function called arithmetic_arranger that formats a list of arithmetic problems vertically and side-by-side, similar to how they are written on paper.

## Features
- Accepts up to 5 arithmetic problems
- Supports addition(+) and subtraction(-)
- Properly aligns numbers for readability
- Optionally displays the answers
- Includes input validation with clear error messages

 ## How It Works 
 
 1. Input
 The function accepts:
    - problems: a list of arithmetic problem strings.
    - show_answers: an optional Boolean value(False by default) 
2. Validation rules
  The function checks for the following errors:
     - more than 5 problems
     - operators other than + or -
     - numbers containing non-digit characters
     - numbers longer than 4 digits
  3. Formatting
     
     Each problem is arranged vertically with:
     - the first number on top
     - the operator and second number below
     - a line of dashes underneath
     - the answer on the last line if requested
     - Determine the width using width = max(len(num1), len(num2)) + 2
     - Right-align numbers using .rjust()
     - Build:
         - top row
         - bottom row
         - dash row
  7. Optional Answer Calculation
     - Execute the code using eval(f"{num1} {operator} {num2}
  8. Combine rows
      - Join problems with 4 spaces
      - Return formatted string
  
