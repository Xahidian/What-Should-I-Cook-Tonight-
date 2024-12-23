# Mini Project 1 – Recipe Recommendation Based on Calorie and Personal Point Ranges.

## Author: Md Hasibul Haque Zahid
## Student ID: 2302302

### Introduction
This project focuses on providing personalized recipe recommendations based on calorie and Weight Watchers personal point ranges. The data for this project was scraped from the [Skinnytaste](https://www.skinnytaste.com) website using **BeautifulSoup**, a powerful web scraping library in Python.

The scraped data includes detailed recipe information such as dish names, calorie counts, personal points, images, and recipe summaries. The primary goal of the project is to assist users in answering the question, "What should I cook tonight?" by providing tailored recipe suggestions that match their dietary preferences.

### Data Collection
Using BeautifulSoup, the first 50 pages of recipes from the Skinnytaste website were parsed, and the following data points were extracted:

- **Dish Name**: The title of the recipe.
- **Image URL**: A link to an image of the dish.
- **Calories**: The number of calories per serving.
- **Personal Points**: Weight Watchers points associated with the recipe.
- **Summary**: A brief description of the dish.
- **Recipe Key**: A feature for filtering recipes (e.g., vegan, gluten-free).

The data was stored in a Pandas DataFrame and exported to a CSV file for further analysis and visualization.

### Data Analysis
#### Key Insights
- **Calorie Distribution**: Most recipes have less than 500 calories, with a few higher-calorie outliers.
- **Personal Points**: Recipes are generally suitable for Weight Watchers, with points ranging from 2 to 10.
- **Recipe Categories**: Recipes are categorized by features like vegan, gluten-free, and more, aiding user preference filtering.

Visualizations were created to better understand calorie ranges, personal points, and recipe categories.

### Features for Users
Users can interact with the program by inputting:

1. **Calorie Range**
2. **Personal Point Range**

The program then recommends up to 10 recipes matching the criteria, displaying:

- Dish Name
- Calorie Count
- Recipe Summary
- Link to Recipe Image

### Challenges and Solutions
- **Pagination Issues**:
  - **Problem**: Navigating through multiple pages was complex due to dynamic pagination.
  - **Solution**: URLs for subsequent pages were programmatically constructed to automate navigation.
  
- **Inconsistent Data Structure**:
  - **Problem**: Missing or incomplete data fields caused errors during scraping.
  - **Solution**: Implemented error handling to skip or log incomplete records.

## Technologies Used
- Python
- Jupyter Notebook
- BeautifulSoup
- Pandas
- Matplotlib

## Report
A detailed report on the project is available [Here](https://github.com/Xahidian/What-Should-I-Cook-Tonight-/blob/main/MiniProject1Zahid.pdf). It provides a comprehensive overview of the scraping process, data analysis, and insights.

## Contact
If you have any questions or would like to discuss the project further, feel free to reach out to me.  
Thank you for visiting my Project!
