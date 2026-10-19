# febrile-seizure-log-analyzer

## Questions
Based off of simulated data of 8 made up records, used to build and test the analysis:
1) What is the average fever for simple seizures?
2) What is the highest fever among simple seizures?
3) What is the average age (in months) for simple seizures?
4) How many seizures in the log are complex (longer than 15 minutes)?
5) How does the average fever compare between simple and complex seizures?
## Data
- Built a simulated dataset of 8 seizure records in Python, stored as a list of dictionaries
- Each record has a patient ID, age in months, fever in celsius (°C), and seizure length in minutes
## Classification 
- Simple: 15 minute or less (<= 15)
- Complex: longer than 15 minutes (> 15)
- Duration was the only criterion
## Analysis
- Used 'for' loops 'if' conditions to sort records into simple and complex groups
- Collected values from each group into lists with '.append()'
- Averages: sum() / len(), rounded to 2 decimals (Q1,Q3,Q5)
- Count: len() of the complex list (Q4)
- Highest value: max() of the complex list (Q2)
- Comparison: looked at the two group averages side by side. It was descriptive only with no statistical test
## Results
- Average fever for simple seizures: 39.76°C
- The highest temperature among simple seizures: 41.1°C
- The average age in months for simple seizures: 16.6 months old
- How many seizures are complex: 3 (P03, P06, P07)
- Fever comparison between simple and complex seizures: simple- 39.76°C complex- 39.97°C
Complex seizures averaged about 0.2 °C higher than simple ones. That difference is small, and with 8 made-up records it can’t show anything real. The point of this project was to build a working analysis pipeline
## Verification
- Worked out each answer by hand and checked that the code's output matched
## Limitations 
- Real complex febrile seizures can also be focal or recur within 24 hours
- Simulated data and small population sample
## Tools
- Python in Google Colab, using no extra libraries: only built-in Python
