# arithmetic-formatter-project
This project contains a Python function called arithmetic_arranger that formats a list of arithmetic problems vertically and side-by-side, similar to how they are written on paper.

## Features
- Accepts up to 5 arithmetic problems.
- Supports addition(+) and subtraction(-).
- Properly aligns numbers for readability.
- Optionally displays the answers.
- Includes input validation with clear error messages.

 ## How It Works 
 
 1. Input
    
 The function accepts:
 
    - problems: a list of arithmetic problem strings.
    
    - show_answers: an optional Boolean value(False by default) 
    
2. Validation rules
   
  The function checks for the following errors:
     - More than 5 problems
     - Operators other than + or -
     - Numbers containing non-digit characters
     - Numbers longer than 4 digits
     
  4. Formatting
     
     Each problem is arranged vertically with:
     - The first number on top
     - The operator and second number below
     - A line of dashes underneath
     - The answer on the last line if requested
     - Determine the width using:
        width = max(len(num1), len(num2)) + 2
     - Numbers are right-aligned using:
        .rjust()
     - Build:
         - top row
         - bottom row
         - dash row
  5. Optional Answer Calculation
     - The result is calculated using:
        eval(f"{num1} {operator} {num2}")
  4. Combine rows
      - Problems are joined with 4 spaces.
      - The formatted string is returned.
        
  ## Skills Practised

     - Functions
     - Lists
     - Loops
     - Conditional statements
     - String methods
     - String formatting with rjust()
     - Input validation
     - Building formatted output

  ## Installation
  Make sure Python is installed. Then run your script normally.

  ## Author

  Created by Unathi Malangabi.

  
