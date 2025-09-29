# Gumi Industrial Energy Consumption Competition

This project focuses on analyzing and forecasting energy consumption for various buildings and factories within the Gumi National Industrial Complex, Korea. The goal is to advance research in industrial energy analytics and support initiatives for smarter, more sustainable facilities.

## Data Preprocessing Steps:

- **Data Loading**
The dataset is loaded from a CSV file (Hanwha Main_data.csv) into a Pandas DataFrame.
- **Datetime Handling**
Combines date and hour columns into a single datetime column.
Converts the datetime column to a proper datetime format using pd.to_datetime.
Drops unnecessary columns like date, hour, and company.
- **Reordering Columns**
Reorders the DataFrame to place datetime as the first column and consumption as the second.
- **Sorting and Indexing**
Sorts the DataFrame by the datetime column.
Checks the DataFrame index for consistency.
- **Visualization**
Plots the consumption column to visualize trends.
Filters and plots consumption values below a threshold (e.g., 40).
- **Smoothing**
Applies a rolling mean (moving average) to the consumption column to create a smoothed_consumption column.
Visualizes the smoothed data.
- **Scaling**
Scales the smoothed_consumption column using MinMaxScaler to normalize values between 0 and 1.
- **Sequence Creation**
Prepares the data for time-series forecasting by creating sequences of past values (X) and corresponding target values (y).
- **Train-Test Split**
Splits the data into training and test sets, ensuring no shuffling to preserve temporal order.

## Key Objectives

- Understand energy consumption trends across sites and time periods.
- Build predictive models for short-term and long-term industrial energy demand.
- Extract interpretable insights that support smart industry and low-carbon goals.

## Results

<img width="1608" height="335" alt="image" src="https://github.com/user-attachments/assets/c0c98076-ff01-485e-86a4-58d3c647722f" />


***
