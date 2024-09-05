# Airbnb Data Analysis

This project analyzes Airbnb listings across various regions of the USA, focusing on key metrics such as price distribution, room types, reviews, and availability. Additionally, the project implements machine learning models to predict certain aspects of Airbnb listings.

## Project Structure

- **Data Loading**: Load Airbnb datasets from multiple regions.
- **Data Processing**: Clean and preprocess the data, including splitting and transforming columns.
- **Exploratory Data Analysis (EDA)**: Visualize key insights such as price distribution, room types, and reviews.
- **Outlier Removal**: Detect and remove outliers based on the z-score.
- **Machine Learning Models**: Use models like RandomForest to predict features like room types.
- **Comparative Analysis**: Compare key metrics across different regions (East, Central, West).

## Dataset
The dataset consists of Airbnb listings from the following regions:
- **East**: Boston (MA), Cambridge (MA), Jersey City (NJ), New York City (NY), Rhode Island (RI), Washington (DC).
- **Central**: Austin (TX), Chicago (IL), Columbus (OH), Dallas (TX), Twin Cities (MS).
- **West**: Denver (CO), Hawaii (HI), Los Angeles (CA), Oakland (CA), San Diego (CA), San Francisco (CA), Seattle (WA).

## Key Features of the Analysis

1. **Data Cleaning**: The script processes raw data, cleans it, and handles missing values.
2. **Outlier Removal**: A function is provided to remove outliers based on z-scores.
3. **Price vs Rating Analysis**: A scatter plot to visualize the relationship between Airbnb listing prices and their ratings.
4. **Comparative Metrics**: Comparison of regions based on:
   - Average Price
   - Room Type Distribution
   - Number of Reviews
   - Availability Trends
5. **Correlation Analysis**: A heatmap to visualize the correlation between various features.
6. **Machine Learning Models**: Predict room types using RandomForest and visualize feature importance.

## Heatmap Visualization
The project also uses Folium to create heatmap visualizations of Airbnb listing locations based on price.

## Requirements

To run this project, you need to install the following libraries:

```bash
pip install pandas matplotlib seaborn scikit-learn folium
```
Running the Project
Clone the repository.
Ensure the datasets are in the correct location (update the file paths in the script).
Run the script to load, process, and analyze the data.
Example Usage

# Load and process the data
combined_df_east = process_and_display_data(file_paths_east)

# Perform analysis and visualize results
analyze_price_vs_rating(filtered_west, 'West')
