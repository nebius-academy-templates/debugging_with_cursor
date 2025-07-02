# Lesson 5: Debugging with Cursor

## Overview
This lesson demonstrates how to effectively debug Python code using Cursor. You'll learn to identify common errors and fix them systematically.

## Setup
1. Install required packages:
   ```
   pip install -r requirements.txt
   ```

## Files Structure
- `sample_sales_data.csv` - Sample data file for analysis
- `brokencode/sales_analyzer.py` - Deliberately broken code with 8 common errors
- `fixedversion/sales_analyzer.py` - Fixed version with explanations

## How to Use This Lesson
1. First, try running the broken code: `python brokencode/sales_analyzer.py`
2. Observe the errors and use Cursor to help debug them
3. Compare with the fixed version to understand the solutions

## Common Errors Demonstrated
1. Wrong file format assumption (Excel vs CSV)
2. Incorrect column names
3. Logic errors in calculations
4. Missing variables
5. File not found errors
6. Division by zero issues
7. Missing function parameters
8. Undefined variables 
