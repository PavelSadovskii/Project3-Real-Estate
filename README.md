# Project Description

This project involves the analysis of advertisements for the sale of apartments in St. Petersburg and neighboring settlements using data from the Yandex.Realty service. The goal is to determine the market value of real estate and set parameters for building an automated system to track anomalies and fraudulent activity in real estate ads.

## Project Goal

The main objective is to establish the parameters for an automated system that can determine the market value of apartments based on user-entered data and automatically obtained cartographic data. This system will help identify anomalies and fraudulent activity in real estate ads.

## Tools and Libraries

The following tools and libraries were utilized for this project:

- Python
- Pandas
- NumPy
- Matplotlib
- Stemming (NLTK SnowballStemmer)

## Data Preprocessing

### Handling Missing Values

- The dataset contained missing values in various columns, which were filled or replaced as appropriate.
- Columns related to apartment type, ceiling height, presence of balconies, and distances to parks and water bodies had significant gaps.
- Data for apartments' proximity to city centers, airports, and other landmarks were filled with appropriate values.

### Data Type Conversion

- The 'locality_name' column was converted to string data type to facilitate handling.
- The 'first_day_exposition' column was converted to a datetime format for further analysis.

### Duplicate Handling

- Implicit duplicates in the names of settlements were eliminated.
- A new column, 'locality_name_changed,' was created with names without duplicates.

### Outlier Handling

- Outliers in columns like 'last_price,' 'total_area,' 'kitchen_area,' 'living_area,' and 'ceiling_height' were handled using the Interquartile Range (IQR) method.

## Exploratory Data Analysis (EDA)

### Data Visualization

- Histograms and scatter plots were created to visualize various aspects of apartment data, including total area, living area, kitchen area, price, number of rooms, ceiling height, floor type, number of floors, distances to city centers, airports, parks, and water bodies.
- The EDA revealed insights into the distribution of apartments based on these parameters.

## Price Analysis

- The project analyzed the factors influencing the total price of apartments, such as total area, living area, kitchen area, number of rooms, floor type, and price per square meter.

## Geographic Analysis

- The average price per square meter for apartments in St. Petersburg was calculated based on their distance from the city center. The analysis revealed a clear trend of decreasing prices with increasing distance from the center.

## General Conclusion

The project successfully preprocessed and analyzed real estate data from Yandex.Realty, allowing for insights into factors affecting apartment prices and geographic trends in pricing. The findings contribute to the development of an automated system for determining market values and identifying fraudulent real estate ads.
