# Netflix Data Cleaning and Visualization Project

## About the Project

In this project, I worked on a Netflix dataset to understand how raw data can be cleaned, processed, analyzed, and converted into useful information.

I used Python and different libraries to find problems in the dataset such as duplicate records, missing values, and data that needed to be converted into a better format.

After cleaning the data, I used different graphs to understand the dataset and find some useful patterns.

---

## What I Wanted to Learn

Through this project, I wanted to understand:

- How to work with a real dataset
- How to find and remove duplicate data
- How to handle missing values
- How to check and change data types
- How to process columns for analysis
- How to use Pandas for data analysis
- How to create graphs using Matplotlib and Seaborn
- How to understand information from graphs
- How to present data in a simple and understandable way

---

## Dataset

The dataset contains information about Netflix movies and TV shows.

Some of the important columns are:

- `show_id` - ID of the title
- `type` - Movie or TV Show
- `title` - Name of the movie or TV show
- `director` - Director name
- `country` - Country
- `release_year` - Release year
- `rating` - Content rating
- `duration` - Movie duration or number of seasons
- `listed_in` - Genre/category
- `date_added` - Date when the title was added

I also created two new columns while cleaning the data:

- `duration_value`
- `duration_unit`

These helped me analyze movie duration and TV show seasons separately.

---

## Data Cleaning

First, I checked the dataset and tried to understand its structure.

During the cleaning process, I found **2 duplicate records**, which I removed.

I also found some missing values:

- 3 missing values in `director`
- 1 missing value in `country`
- 1 missing value in `rating`
- 1 missing value in `date_added`

For `director`, `country`, and `rating`, I used `Unknown` instead of removing the complete rows because the other information in those records was still useful.

I converted the `date_added` column into a proper datetime format.

The `duration` column contained both movie durations and TV show seasons. So I separated the numerical value and the unit into two different columns.

For example:

`120 min` → `120` and `min`

`3 Seasons` → `3` and `Seasons`

I also checked the numerical values for unusual values or possible outliers.

---

## Data Analysis and Visualizations

After cleaning the data, I created different visualizations to understand it better.

### 1. Movies vs TV Shows

I compared the number of Movies and TV Shows in the dataset.

The dataset contains:

- 7 Movies
- 5 TV Shows

So, there are more Movies than TV Shows in this dataset.

### 2. Content by Country

I checked which countries had the most titles.

India had the highest number of titles with 5, followed by the USA with 3 and the UK with 2.

### 3. Content by Release Year

I analyzed how the titles were distributed across different release years.

The dataset contains titles released between 2018 and 2023.

### 4. Content by Genre

I checked the different genres available in the dataset.

Drama and Documentary were the most common genres, with 2 titles each.

### 5. Content by Rating

I analyzed the ratings of the titles.

PG-13 was the most common rating with 3 titles.

### 6. Movie Duration

I analyzed the duration of the movies separately from TV shows.

The movie durations ranged from 95 to 145 minutes.

The longest movie was **Future Earth** with 145 minutes, while **Mystery House** was the shortest with 95 minutes.

### 7. Release Trend

I also created a line graph to understand how the number of titles changed across different release years.

---

## Tools and Libraries Used

For this project, I used:

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## What I Learned

While working on this project, I learned that data analysis is not only about creating graphs.

Before making visualizations, the data needs to be checked and cleaned properly.

I learned how to:

- Work with CSV files
- Explore a dataset using Pandas
- Find duplicate records
- Handle missing values
- Work with dates
- Create new columns from existing data
- Analyze categorical and numerical data
- Create different types of visualizations
- Find useful information from graphs

This project also helped me understand the basic workflow of a data analysis project:

**Raw Data → Cleaning → Processing → Analysis → Visualization → Insights**

---

## Project Files

```text
Netflix_Data_Cleaning_Project/
│
├── netflix_data_cleaning_project.csv
├── netflix_cleaned_data.csv
├── Netflix_Data_Cleaning_Visualization.ipynb
└── README.md


## Conclusion

This was one of my practical projects for learning data analysis.

I started with a raw Netflix dataset and worked step by step to clean the data, process it, analyze it, and create visualizations.

The project helped me understand how Python can be used to convert raw data into information that is easier to understand.

It also gave me practical experience with Pandas, Matplotlib, Seaborn, and Jupyter Notebook.