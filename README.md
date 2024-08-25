
<h1 align="center">Data Engineering: Data Cleaning Beginner's Guide<p align="center"></h1>

<h1 align="center">Bar Bettash<p align="center">
<a href="https://www.linkedin.com/in/barbettash/" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="LinkedIn" height="30" width="40" /></a>
</h1>


<!-- ABOUT THE PROJECT -->
## About The Project

This project demonstrates fundamental data cleaning techniques using Python. The dataset used in this project contains various types of "noise" and missing values that need to be addressed before performing any data analysis or building machine learning models. Below, we outline the main issues identified in the dataset and the corresponding solutions implemented.

## Dataset

Thanks to Github User ' trentpark8800 ' for the data and walkthrough. 

### Built With

Python <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a>

![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a>

![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) <a href="https://matplotlib.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/matplotlib/matplotlib-original.svg" alt="matplotlib" width="40" height="40"/> </a>


## Important Note on Data Cleaning

- It's important to remember the reason for data cleaning: the context in which the data will be used. 
- For instance, when dealing with date and stock price data, one might consider using a machine learning model to predict missing values. 
- However, if the missing prices occur over weekends, the predictions could be inaccurate since the market is closed. 
- In such cases, the best approach is to carry forward the last known price until the market opens again.


<!-- GETTING STARTED -->
## Getting Started


### Prerequisites

To run the project, you need the following libraries installed:

* pandas: A powerful library for data manipulation, analysis, and loading data from various sources (CSV in this case).
  ```sh
  pip install pandas

* numpy: Provides efficient operations on numerical data (arrays, matrices).
  ```sh
  pip install numpy

* matplotlib: Used for creating static visualizations like histograms and scatterplots to explore data.
  ```sh
  pip install matplotlib


## Project Overview

Data cleaning is an essential step in the data engineering pipeline. The quality of the data directly impacts the performance of any analytical or machine learning model. This project covers several key data cleaning tasks:

1. **Handling Missing Values**:
   - Removed rows with missing `Client` names since they represent incomplete data that cannot be reliably inferred.
   - Imputed missing values in the `AmountUSD` column using the mean, which was determined to have the smallest error compared to the median.
   - Replaced missing values in the `ClientTier` column with the most frequent category (`mode`).

2. **Removing Duplicates**:
   - Identified and removed duplicate rows based on all columns except for `TransactionID`, ensuring that each transaction is unique.

3. **Standardizing Text Data**:
   - Cleaned `Client` and `Beneficiary` names by removing uneven characters and standardizing all text to uppercase, ensuring consistency across the dataset.

4. **Cleaning Numeric Data**:
   - Replaced null values in the `AmountUSD` column with the mean, following an error analysis that indicated this approach introduced the least distortion.

5. **Imputing Categorical Values**:
   - Replaced missing values in the `ClientTier` column with the most frequent value (`mode`), ensuring that each client has a valid tier classification.
  

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.


<!-- CONTACT -->
## Contact

<p align="left">
<a href="https://www.linkedin.com/in/barbettash/" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="https://www.linkedin.com/in/barbettash/" height="30" width="40" /></a>
</p>


**bar.bettash.jobs@gmail.com** 


<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

This code is provided "as is" and may not function as intended in the future due to potential updates to external libraries, frameworks, websites, or APIs it interacts with. The code is no longer actively maintained and may require modifications to adapt to future changes.

**Recommendations:**

* Keep an eye on updates to libraries and dependencies to ensure compatibility.
* Be prepared to adapt the code based on future changes in the target website or API.
