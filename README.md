# Exploratory-Data-Analysis-on-YouTube-Data-Using-Python

## Project Overview

This project aims to perform Exploratory Data Analysis (EDA) on a YouTube dislikes dataset. The dataset contains data about YouTube trending videos from August 2020 to December 2021, including video information such as views, likes, dislikes, comments, and metadata for videos from the USA, Canada, and Great Britain.

## Objective

The primary goal of this analysis is to uncover insights from Youtube Dislikes Dataset using EDA. **NumPy**, a popular data manipulation tool, and **Pandas**, a popular data analysis library used to perform analysis on the data. For data visualization, the **Matplotlib** and  **Seaborn** libraries are used. 

## Dataset Information

- **Source:** [YouTube Dislikes Dataset on Kaggle](https://www.kaggle.com/datasets/dmitrynikolaev/youtube-dislikes-dataset)
  
**Data Columns**:

| Column Name      | Description                                                        |
|------------------|--------------------------------------------------------------------|
| `Video ID`       | Unique identifier for the video.                                   |
| `Title`          | Title of the video.                                                |
| `Channel ID`     | Unique identifier for the YouTube channel.                         |
| `Channel Title`  | Name of the YouTube channel.                                       |
| `Published at`   | Date and time when the video was published.                        |
| `View count`     | Total views of the video.                                          |
| `Likes`          | Number of likes the video received.                                |
| `Dislikes`       | Number of dislikes the video received.                             |
| `Comment Count`  | Number of comments on the video.                                   |
| `Tags`           | Tags associated with the video.                                    |
| `Description`    | Description of the video.                                          |
| `Comments`       | List of comments on the video.                                     |


## Steps Involved in the Project

### 1. Data Import and Overview
- Import necessary libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`).
- Read the dataset and display the first 5 and last 5 records for an initial view.

### 2. Dataset Information and Shape
- Checked the structure and data types of the dataset.
- Figured the shape of the dataset and understood how the data is distributed.

### 3. Handle Missing Values
- Identified null values in each column of the dataframe.

### 4. Statistical Summary
- Generated statistical summaries for both numerical and categorical columns.
- Provide insights into key metrics such as average likes, dislikes, and views.

### 5. Convert Datetime Column
- Converted the `Published at` column from an object to pandas datetime.

### 6. Extract Month from Published Date
- Created a new column `published_month` that contains the month the video was published.

### 7. Map Month Numbers to Names
- Replaced numerical month values with month names (e.g., 1 becomes 'Jan', 2 becomes 'Feb').

### 8. Monthly Video Count
- Counted the number of videos published each month.
- Sorted the months based on video count in descending order.

### 9. Unique Count Analysis
- Figured out, number of unique `video_id`, `channel_id`, and `channel_title`.

### 10. Active Channels Analysis
- Identified the top 10 channels with the highest number of videos and the bottom 10 channels with the least number of videos.

### 11. Likes Analysis
- Identified the video with the maximum and minimum likes.

### 12. Dislikes Analysis
- Identified the video with the maximum and minimum dislikes.

### 13. Views vs Dislikes Correlation
- Established the relationship between video views and the number of dislikes.
- Used a correlation matrix to visualize the correlation.

### 14. January Video Analysis
- Retrieved all information about videos published in month January.
- Counted number of videos published in month January.

## Results and Insights

After performing the EDA, the following insights were derived:

### 1. Top/Bottom Videos:
- identified videos with the maximum and minimum likes and dislikes, revealing the engagement patterns.

### 2. Impact of Views on Dislikes:
- The correlation between views and dislikes is 0.68, indicate that increase in view count leads to increase of dislikes count.

