# Airbnb Data Analysis Project

This project focuses on cleaning and analyzing an Airbnb dataset using Python.  
The goal was to understand the data, remove inconsistencies, and explore patterns related to room types, neighbourhood groups, pricing, and reviews.

## Dataset

- Original file: `Airbnb_Open_Data.xlsx`
- Converted to: `airbnb_data.csv`
- Final cleaned records: **83,390 rows**
- Total features after cleaning: **24 columns**

The dataset contains information about Airbnb listings such as location, room type, price, service fee, reviews, and availability.

## Tools and Libraries Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Plotly (for interactive visuals)

## Data Cleaning Steps

The following steps were performed to prepare the data:

1. Converted the Excel file to CSV format
2. Removed duplicate rows (541 duplicates found)
3. Dropped unnecessary columns:
   - `house_rules`
   - `license`
4. Cleaned monetary columns (`price`, `service fee`) by:
   - Removing `$` and commas
   - Converting them to numeric values
5. Renamed columns:
   - `price` → `price $`
   - `service fee` → `service_fee $`
6. Removed rows with missing values
7. Converted data types:
   - IDs converted to string
   - Dates converted to datetime
   - Construction year converted to integer
8. Standardized column names to lowercase

After cleaning, the dataset was consistent and ready for analysis.

## Exploratory Data Analysis (EDA)

### Room Type Distribution
- Entire home/apartment: **44,162**
- Private room: **37,474**
- Shared room: **1,646**
- Hotel room: **108**

Visualizations included bar charts, line plots, and histograms.

### Neighbourhood Group Distribution
- Brooklyn: **34,621**
- Manhattan: **34,561**
- Queens: **11,124**
- Bronx: **2,267**
- Staten Island: **816**

Brooklyn and Manhattan have the highest number of listings.

### Reviews Analysis

- Verified hosts have slightly higher average review ratings than unverified hosts.
- Review rate was compared across:
  - Neighbourhood groups
  - Room types
  - Host verification status

Boxplots and bar charts were used to visualize these trends.

### Availability vs Listings

- A regression plot was created between:
  - `calculated host listings count`
  - `availability 365`
- Correlation value: **0.13**

This shows a weak positive relationship between the number of listings a host owns and availability.

## Key Insights

- Entire homes and private rooms dominate the market.
- Brooklyn and Manhattan are the most active areas.
- Verified hosts generally receive better reviews.
- Availability is not strongly dependent on the number of listings owned by a host.

## Project Purpose

This project was done to practice:
- Data cleaning techniques
- Exploratory data analysis
- Working with large real-world datasets
- Creating meaningful visualizations
- Extracting insights from data

## How to Run

1. Clone the repository
2. Install required libraries
3. Run the notebook or Python script step by step

## License

This project is created for learning and educational purposes.  
The dataset belongs to its original source.

