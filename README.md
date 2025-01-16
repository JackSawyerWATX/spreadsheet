# Spreadsheet Functions Project

This project implements a custom spreadsheet functionality using JavaScript, allowing the evaluation of mathematical expressions and the application of predefined functions within spreadsheet-style cells.

## Features

1. **Mathematical Operations:**
   - Supports addition (`+`), subtraction (`-`), multiplication (`*`), and division (`/`) with precedence handling.

2. **Custom Spreadsheet Functions:**
   - `sum`: Calculates the sum of numbers.
   - `average`: Calculates the average of numbers.
   - `median`: Calculates the median of numbers.
   - `even`: Filters even numbers.
   - `someeven`: Checks if some numbers are even.
   - `everyeven`: Checks if all numbers are even.
   - `firsttwo`: Returns the first two numbers.
   - `lasttwo`: Returns the last two numbers.
   - `has2`: Checks if the number 2 exists in the list.
   - `increment`: Increments all numbers by 1.
   - `random`: Generates a random number within a range.
   - `range`: Generates a range of numbers.
   - `nodupes`: Removes duplicates from the list.

3. **Cell Range Evaluation:**
   - Supports cell range references (e.g., `A1:C3`).
   - Dynamically calculates the values of referenced cells.

4. **Dynamic UI:**
   - Creates a grid layout with cells labeled from `A1` to `J99`.
   - Cells are editable and support formula evaluation.

## Technologies Used

- **JavaScript**: Core language for functionality.
- **HTML**: Markup for the grid layout and input elements.
- **CSS**: (Optional) Styling for grid layout and labels.

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the project directory:
   ```bash
   cd spreadsheet-functions
   ```
3. Open the `index.html` file in a web browser.

## Usage

1. Open the project in a browser.
2. Enter values or formulas in the cells. Formulas should start with an `=` (e.g., `=A1+B1`).
3. Supported cell references include individual cells (e.g., `A1`) and ranges (e.g., `A1:C3`).
4. Use spreadsheet functions by typing their names (e.g., `=sum(1,2,3)`).

## Project Structure

- `index.html`: Contains the grid layout and input elements.
- `main.js`: Implements the core logic for evaluating expressions and updating cell values.
- `style.css` (optional): Contains styling for the grid and labels.

## Code Overview

### Core Functions

- `infixEval`: Evaluates infix mathematical operations based on precedence.
- `highPrecedence`: Handles high precedence operators (`*`, `/`).
- `applyFunction`: Evaluates custom spreadsheet functions from string input.
- `evalFormula`: Parses and evaluates formulas with support for cell references and ranges.
- `update`: Handles cell value changes and triggers formula evaluation.

### Utility Functions

- `range`: Generates an array of numbers within a specified range.
- `charRange`: Generates a range of characters.
- `isEven`, `sum`, `average`, `median`: Provide various mathematical utilities.

### UI Initialization

- Dynamically generates a grid layout with labeled rows and columns.

## Future Improvements

- Add support for additional functions (e.g., `max`, `min`).
- Enhance error handling for invalid inputs and circular references.
- Implement better styling for a user-friendly interface.
- Extend range support to larger grids.

---

Feel free to contribute or suggest improvements!
