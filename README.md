# Quadratic Equation Solver & Grade Converter

A single-file web application that solves quadratic equations and converts numeric scores to letter grades.

## Features

### 1. Quadratic Equation Solver
- Solves equations in the form: ax² + bx + c = 0
- Calculates discriminant (D = b² - 4ac)
- Determines nature of roots:
  - Two distinct real roots (D > 0)
  - One real repeated root (D = 0)
  - Two complex conjugate roots (D < 0)
- Input validation ensures coefficient 'a' cannot be zero

### 2. Grade Converter
- Converts numeric scores (0-100) to letter grades using the exact scale:
  - A+: 85–100
  - A: 75–84
  - B+: 65–74
  - B: 60–64
  - C+: 55–59
  - C: 50–54
  - D: 0–49
- Input validation ensures scores are between 0 and 100

## How to Run

1. Download the file: Save `index.html` to your local machine
2. Open in browser: Double-click the `index.html` file to open it in your default web browser
3. Use offline: The application runs completely offline - no internet connection required

### Alternative Methods:
- Drag and drop the `index.html` file into an open browser window
- Right-click the file and select "Open with" → Choose your preferred browser

## Test Cases

### Quadratic Equation Solver Test Cases:

1. Two real roots (D > 0):
   - Input: a=1, b=-3, c=2
   - Expected: Roots: x₁ = 2, x₂ = 1

2. One real root (D = 0):
   - Input: a=1, b=-4, c=4
   - Expected: Root: x = 2 (repeated)

3. Complex roots (D < 0):
   - Input: a=1, b=2, c=5
   - Expected: Complex conjugate roots

4. Validation test:
   - Input: a=0, b=2, c=3
   - Expected: Error message for coefficient a

### Grade Converter Test Cases:

1. Edge cases:
   - Input: 85 → Expected: A+
   - Input: 75 → Expected: A
   - Input: 65 → Expected: B+
   - Input: 60 → Expected: B
   - Input: 55 → Expected: C+
   - Input: 50 → Expected: C
   - Input: 49 → Expected: D

2. Boundary values:
   - Input: 100 → Expected: A+
   - Input: 0 → Expected: D

3. Mid-range values:
   - Input: 92 → Expected: A+
   - Input: 80 → Expected: A
   - Input: 70 → Expected: B+
   - Input: 62 → Expected: B
   - Input: 57 → Expected: C+
   - Input: 52 → Expected: C
   - Input: 30 → Expected: D

## File Structure