

# MovieLens: Deep Dive into User Ratings & Movie Trends

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-1.3+-orange.svg)
![NumPy](https://img.shields.io/badge/NumPy-1.21+-yellow.svg)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.5+-green.svg)
![Seaborn](https://img.shields.io/badge/Seaborn-0.11+-red.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## Project Overview

This project analyzes the MovieLens dataset to understand movie rating patterns, genre preferences, and user behavior. The goal is to extract valuable insights that can help improve user engagement and overall experience for movie recommendation platforms. By examining relationships between movies, users, and ratings, we identify key trends that drive user satisfaction and content consumption.

## Business Problem

Movie recommendation platforms face challenges in:
- Understanding genre preferences across diverse user segments
- Identifying high-quality content that resonates with users
- Optimizing recommendation algorithms based on rating patterns
- Tailoring user experience based on demographic differences

This analysis addresses these challenges by uncovering hidden patterns in movie ratings and user behavior.

## Dataset Description

The analysis utilizes three primary datasets:

| Dataset | Description | Key Fields |
|---------|-------------|------------|
| **movies.csv** | Contains information about movies and their genres | movie_id, title, genres |
| **users.csv** | Contains demographic information about users who rated movies | user_id, gender, age, occupation, zip_code |
| **ratings.csv** | Contains actual ratings given by users to particular movies | user_id, movie_id, rating, timestamp |

**Dataset Characteristics**:
- **Movies**: 3,883 unique titles across 18 genres
- **Users**: 6,040 unique users with demographic information
- **Ratings**: 1,000,209 individual movie ratings
- **Rating Scale**: 1-5 stars (whole numbers only)

## Key Findings

### 1. **Movie Genre Analysis**
- **Genre Diversity**: The dataset spans **18 distinct genres** of films
- **Top 5 Genres** by number of movies:
  1. Drama (1,603 movies)
  2. Comedy (1,200 movies)
  3. Action (503 movies)
  4. Thriller (492 movies)
  5. Romance (471 movies)
- **Multi-Genre Classification**: **50% of movies** are classified under multiple genres
- **Genre Performance**:
  - **Film-Noir** has the highest average rating (3.92/5)
  - **Fantasy** has the lowest average rating (3.21/5)
  - **72% of genres** have an average rating above 3.5

### 2. **Top-Rated Movies**
- **Highest-Rated Movies** (all with perfect 5.0 ratings):
  - "Great Day in Harlem, A"
  - "Prefontaine"
  - "Saint of Fort Washington, The"
  - "They Made Me a Criminal"
  - "Someone Else's America"
- **Lowest-Rated Movies** (all with 1.0 ratings):
  - "Shadow of Angels (Schatten der Engel)"
  - "Power 98"
  - "Three Lives"
  - "Menace II Society"
  - "Daens"
- **Frequently-Rated Movies**:
  - 334 movies received more than 100 ratings
  - "Close Shave, A" achieved the highest average rating (4.49/5) among frequently-rated movies (112 ratings)
  - "Star Wars" received the most ratings (583 ratings) while maintaining an excellent 4.35/5 average

### 3. **User Demographics and Behavior**
- **Gender Distribution**: 
  - 71% male users
  - 29% female users
- **Rating Patterns by Gender**:
  - Average ratings by gender are nearly identical (approximately 3.53/5)
  - Both genders show similar genre preferences
- **Occupation-Based Insights**:
  - Non-working users tend to give higher ratings than working professionals
  - Healthcare workers give the lowest average ratings (3.39/5)
  - Retired users give the highest average ratings (3.70/5)
- **Age-Based Patterns**:
  - Younger users (under 18) give the most generous ratings (3.78/5)
  - Middle-aged users (35-44) give the most critical ratings (3.44/5)

### 4. **Rating Distribution Analysis**
- **Overall Rating Distribution**:
  - Mean rating: 3.53/5
  - Most common rating: 4/5 (34% of all ratings)
  - Least common rating: 1/5 (6% of all ratings)
- **Rating Extremes**:
  - 5.5% of movies have an average rating below 2.5
  - 9.1% of movies have an average rating above 4.0
- **Rating Consistency**:
  - Movies with more ratings tend to have more stable average ratings
  - Newly released movies show higher rating variability

## Methods Used

### 1. **Data Preprocessing**
- **Data Integration**: Merged three datasets using movie_id and user_id as keys
- **Missing Value Handling**: Verified completeness of all datasets
- **Data Type Conversion**: Optimized data types for efficient processing
- **Feature Engineering**: Created derived metrics like average ratings per genre

### 2. **Exploratory Data Analysis (EDA)**
- **Univariate Analysis**: Examined distributions of ratings, genres, and user demographics
- **Bivariate Analysis**: Explored relationships between genres and ratings, demographics and ratings
- **Multivariate Analysis**: Investigated complex interactions between multiple variables

### 3. **Statistical Analysis**
- **Descriptive Statistics**: Calculated means, medians, and distributions
- **Comparative Analysis**: Compared ratings across genres, demographics, and movie popularity
- **Correlation Analysis**: Identified relationships between numerical variables

### 4. **Data Visualization**
- **Distribution Visualizations**: Histograms, box plots for rating distributions
- **Comparative Visualizations**: Bar charts for genre comparisons, grouped by demographics
- **Relationship Visualizations**: Scatter plots for rating correlations
- **Advanced Visualizations**: Heatmaps for genre co-occurrence patterns

## Technologies

- **Programming Language**: Python 3.8+
- **Data Manipulation**: Pandas 1.3+, NumPy 1.21+
- **Data Visualization**: Matplotlib 3.5+, Seaborn 0.11+
- **Development Environment**: Jupyter Notebook
- **Version Control**: Git

## Project Outcomes

### 1. **Business Impact**
- Identified high-performing genres (Film-Noir, Documentary) for content acquisition
- Discovered underperforming genres (Fantasy, Horror) requiring quality improvement
- Uncovered demographic segments with distinct rating patterns for targeted marketing
- Established baseline metrics for recommendation algorithm performance

### 2. **Technical Contributions**
- Created comprehensive genre preference profiles for user segmentation
- Developed rating consistency metrics for content quality assessment
- Built demographic-based rating prediction framework
- Established data pipeline for continuous movie rating analysis

### 3. **User Experience Enhancements**
- Identified high-quality, less-known movies for discovery features
- Discovered rating patterns to improve recommendation accuracy
- Uncovered demographic preferences for personalized user interfaces
- Established quality thresholds for content curation



## How to Use This Repository

1. **Clone the repository**:
   ```bash
   git clone https://github.com/usamaabidai/MovieLens-Data-Analysis.git
   ```

2. **Navigate to the project directory**:
   ```bash
   cd MovieLens-Data-Analysis
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

5. **Open and execute**:
   - `MovieLens_Data_Analysis.ipynb` for complete analysis
   - Explore individual sections as needed

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Connect

- [LinkedIn](https://www.linkedin.com/in/ucheamaefule/)
- [Portfolio](https://github.com/uamaefule/Data-Analytics-Portfolio)
- [Email](ucheamaefule@ymail.com)

---

*This project demonstrates comprehensive data analysis capabilities in the entertainment domain, showcasing skills in data manipulation, statistical analysis, and visualization. The insights provide actionable recommendations for improving movie recommendation systems and enhancing user experience through data-driven decision making.*
