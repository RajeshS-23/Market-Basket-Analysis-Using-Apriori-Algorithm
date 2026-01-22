# Market Basket Analysis Using Apriori Algorithm

## Overview
This project performs Market Basket Analysis to discover associations between products purchased together.  
Using the Apriori algorithm, the project identifies frequent itemsets and generates association rules based on support, confidence, and lift.

The analysis helps understand customer purchasing behavior and can be used for recommendation systems and sales optimization.

---

## Technologies Used
- Python
- Pandas
- NumPy
- Apyori (Apriori Algorithm)

---

## Dataset
- File name: `Market_Basket_Optimisation.csv`
- Each row represents a single transaction
- Each column represents an item purchased
- Missing or empty values are treated as no purchase

---

## Project Workflow

1. Load the transaction dataset
2. Perform basic data inspection and validation
3. Convert dataset into transaction format required for Apriori
4. Apply Apriori algorithm with defined thresholds
5. Extract association rules
6. Convert results into a structured DataFrame for analysis

---

## Data Preparation
- Each transaction is converted into a list of items
- Items with value `0` are excluded
- Final transaction list is used as input for Apriori

---

## Apriori Algorithm Parameters
- Minimum Support: `0.003`
- Minimum Confidence: `0.2`
- Minimum Lift: `3`
- Rule Length: 2 items

These thresholds help filter only meaningful and strong association rules.

---

## Output
The final output includes:
- Item 1
- Item 2
- Support
- Confidence
- Lift

The results are stored in a Pandas DataFrame for easy interpretation.

---

## Use Cases
- Product recommendation systems
- Cross-selling strategies
- Retail analytics
- Customer behavior analysis

---

## How to Run the Project

1. Install required dependency:
   ```bash
   pip install apyori pandas numpy
