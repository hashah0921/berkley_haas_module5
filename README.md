# README - Project Coupon


## Project Overview
This project is an Exploratory Data Analysis (EDA) investigating the factors that influence whether a driver will accept a coupon delivered to their cell phone while driving. 

Using data visualizations, statistical summaries, and probability distributions, this analysis distinguishes between customers who accepted a driving coupon and those who did not. It serves as a comprehensive portfolio piece demonstrating data cleaning, manipulation, and visualization using Python.

## Data Description
The dataset used in this project originates from the **UCI Machine Learning Repository** and was collected via a survey on Amazon Mechanical Turk. The survey presented users with various driving scenarios and asked whether they would accept a coupon.

The data encompasses three main categories of attributes:
1. **User Attributes:** Gender, age, marital status, education, occupation, annual income, and frequency of visiting bars, coffee houses, and restaurants.
2. **Contextual Attributes:** Driving destination, weather, temperature, time of day, and current passengers (e.g., alone, partner, kids, friends).
3. **Coupon Attributes:** Time before expiration (e.g., 2 hours, 1 day) and coupon type (e.g., Bar, Coffee House, Carry out, Expensive/Cheap Restaurants).

*Target Variable (`Y`):* `1` indicates the user accepted the coupon, and `0` indicates they rejected it.

## Key Deliverables & Investigations
### 1. Data Cleaning and Imputation
- Investigated the dataset for missing and problematic values.
- Imputed missing categorical data using the mode (most frequent value) for the respective columns to preserve dataset integrity.

### 2. General Visualizations
- Calculated the overall acceptance rate across all coupon types.
- Generated bar plots to visualize the distribution of different coupon types.
- Plotted histograms to understand the distribution of temperatures during the driving scenarios.

### 3. Deep Dive: Bar Coupons
A focused investigation was conducted on drivers who received **Bar** coupons to test various hypotheses. Key findings include:
- Acceptance rates were compared between infrequent (<= 3 times/month) and frequent (> 3 times/month) bar-goers.
- Analysis revealed a significantly higher acceptance rate among drivers who frequent bars more than once a month AND are over the age of 25.
- Further analysis confirmed that the ideal demographic for a bar coupon is a driver who goes to bars regularly, does not have children as passengers, and is either younger (under 30) or works outside of farming/fishing/forestry.
- **Hypothesis:** The coupon acts as a successful *nudge* for individuals who already exhibit a social, outgoing lifestyle, provided their immediate context (like not having kids in the car) allows for an impromptu stop.

### 4. Independent Investigation


## Technologies Used
* **Python** (Data processing and analysis)
* **Pandas** (Data manipulation, masking, filtering)
* **Matplotlib & Seaborn** (Data visualization)
* **Jupyter Notebook** (Interactive analysis environment)

## How to Run the Project
1. Clone the repository.
2. Ensure you have the `data/coupons.csv` file in the correct directory.
3. Install the required libraries: `pip install pandas numpy matplotlib seaborn`
4. Run the `assignment5_1.ipynb` notebook cell by cell to reproduce the analysis.
