# TOPSIS Assignment

This project implements the **TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution)** method for multi-criteria decision-making. The tool ranks alternatives based on given weights and impacts of criteria.

## Features
- **Input:** CSV file containing alternatives and criteria.
- **Processing:** 
  - Normalize the decision matrix.
  - Apply weights and impacts to criteria.
  - Calculate distances from ideal best and worst solutions.
  - Rank alternatives based on their closeness to the ideal solution.
- **Output:** A CSV file with TOPSIS scores and rankings.

## How to Use
1. Run the script with the following command:
   ```
   python <program.py> <InputDataFile> <Weights> <Impacts> <ResultFileName>
   ```
   Example:
   ```
   python topsis.py input.csv "1,2,3,4" "+,-,+,+" output.csv
   ```
2. The program validates inputs and generates a ranked output file.

## Prerequisites
- Python 3.x
- Required libraries: pandas, numpy

## File Description
- `input.csv`: Input data file with at least three columns (ID, criteria values).
- `output.csv`: Result file with TOPSIS scores and rankings.

## Notes
- Impacts (`+` for benefit, `-` for cost) and weights must match the number of criteria.
- Ensure numeric values for all criteria columns.

---
