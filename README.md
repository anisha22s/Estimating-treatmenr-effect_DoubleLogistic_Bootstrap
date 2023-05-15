# Hotel Cancellation Analysis

This project focuses on analyzing the impact of assigning a different room on hotel room cancellations. It utilizes the "hotel_cancellation.csv" dataset to estimate treatment effects, measure the effect using double logistic regression, and estimate the standard error using bootstrap.

## Dataset

The dataset used in this project is "hotel_cancellation.csv." It contains information about hotel bookings, including various attributes such as customer demographics, booking details, and whether the booking was canceled or not. The dataset is provided in CSV format and should be downloaded before running the analysis.

## Prerequisites

To run the analysis code, you need to have the following dependencies installed:

- Python 3 (https://www.python.org/)
- pandas (https://pandas.pydata.org/)
- statsmodels (https://www.statsmodels.org/stable/index.html)
- scikit-learn (https://scikit-learn.org/stable/)

You can install the required Python packages by running the following command:

pip install pandas statsmodels scikit-learn


## Analysis Steps

1. Estimating Treatment Effects:
   - The code will load the "hotel_cancellation.csv" dataset.
   - It will use a treatment indicator of "different room is assigned" and all other columns as covariates.
   - The treatment effects will be estimated using a suitable method (e.g., propensity score matching, regression analysis).
   - The results will be interpreted to understand the effect of a different room assignment on room cancellations.

2. Double Logistic Regression:
   - The code will perform double logistic regression to measure the effect of "different room is assigned" on room cancellations.
   - It will use the same dataset and treatment indicator as in the previous step.
   - The regression analysis will account for covariates and estimate the treatment effect.
   - The results will provide insights into the relationship between room assignment and cancellations.

3. Bootstrap for Standard Error Estimation:
   - The code will use the double logistic regression results to estimate the standard error of the treatment effects.
   - It will apply the bootstrap method to generate multiple resamples of the dataset.
   - Each resampled dataset will be used to re-estimate the treatment effects through double logistic regression.
   - The standard error will be calculated based on the variability of the treatment effect estimates across the resamples.

## Running the Analysis

To run the analysis, follow these steps:

1. Download the "hotel_cancellation.csv" dataset and place it in the project directory.

2. Open the code file (e.g., "analysis.py") in a Python IDE or text editor.

3. Ensure that you have installed all the required dependencies listed in the Prerequisites section.

4. Execute the code to perform the analysis.

5. The results will be displayed or saved to a file, depending on the code implementation.

## Conclusion

This project provides insights into the impact of different room assignments on hotel room cancellations. By estimating treatment effects, conducting double logistic regression, and estimating the standard error using bootstrap, we gain a deeper understanding of the relationship between these variables. The findings can help hotels make informed decisions regarding room assignments to minimize cancellations and optimize customer satisfaction.

For further details, refer to the code file and comments within the project repository.

