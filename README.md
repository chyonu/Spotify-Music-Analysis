# Spotify-Music-Analysis
Unlock the Rhythm of Spotify🎵📊 

## Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Recommendations](#recommendations)
- [Limitations](#limitations)

  
### Project Overview
---
Explore the world of Spotify music with my data-driven analysis and interactive charts. Gain insights into trending artists, track popularity, and more. I used MySQL for data analysis and Power BI for dynamic visualizations. 

### Data Sources
---
The Primary dataset used for this analysis is available on [Kaggle](https://www.kaggle.com/datasets/rajatsurana979/most-streamed-spotify-songs-2023).
It contains information about tracks, artists, charts, and other music-related data from Spotify.

### Tools
---
- MySQL
  - Data Cleaning
  - Data Analysis
- PowerBI
  - Creating Visuals
 
### Data Cleaning
---
In the initial data preparation phase, I performed the following tasks:
1. Data loading and inspection.
2. Handling missing values.
3. Handling outliers by transforming them.
4. Data Cleaning and Formatting.
   
### Exploratory Data Analysis
---

EDA involved exploring the spotify-data to answer key questions, such as:
- What are the 10 most popular tracks in terms of streams?
- Which Artists has the most tracks in Spotify playlists?
- What is the overall trend in song release years?
- What track has the highest percentage of danceability?
- What tracks can be found in both Spotify and Apple playlists?
- What is the total number of tracks released in 2023?
- What is the most popular track in terms of streams in 2023?
  
### Data Analysis
---
Data analysis was performed using SQL with MySQL to explore various aspects of the Spotify music data.
The primary objectives were to understand trends in track popularity, artist performance, and danceability within the Spotify platform.
A selection of [interactive](https://app.powerbi.com/reportEmbed?reportId=ee6f6ab8-9e67-4dac-b754-e0fe0c355a8e&autoAuth=true&ctid=a18d4da0-fa29-4ca0-80a3-dafe7e29cff3) visualizations created in Power BI showcases some of the key insights, such as average streams and release year trends.
```sql
-- Handling missing values
UPDATE spotify
SET `key` = 'Unknown'
WHERE TRIM(`key`) = '';
```


### Results
---
The analysis results are summarized as follows:

1. Peru by Ed Sheeran, Fireboy DML had the track with the most danceability with 96%.
2. It was identified that Circles by Post Malone resonated most with Spotify users in terms of streams.
3. The release year had an impact on a track's count, as it was noticed that 2022 had the highest amount of tracks released.
4. Analysis provided insights into tracks' presence in Shazam charts, shedding light on fukumean as the most shazam charts count which was released in 2023.
   
### Recommendations
---
Based on the analysis, I recommend the following actions:

- Given that "Peru" by Ed Sheeran and Fireboy DML had the track with the highest danceability at 96%, consider creating or promoting danceable tracks to engage Spotify users and potentially boost their popularity.
- "Circles" by Post Malone resonated strongly with Spotify users in terms of streams. Focus on promoting tracks with similar characteristics or themes that resonate with your target audience.
- Since 2022 had the highest number of tracks released, consider the timing and competition when releasing new tracks. Strategic release planning can help your music stand out in a crowded market.
- Tracks like "fukumean" with a high presence in Shazam charts can indicate wider recognition and popularity. Explore strategies to increase your tracks' presence on platforms like Shazam to expand your audience reach.
- Collaborations with artists who have a strong presence on Spotify and a loyal fan base can help boost music's visibility and popularity.
  
### Limitations
---

- To handle missing values in key column, imputed data points were introduced. However, these imputed values may not perfectly represent the true data, potentially affecting the accuracy of the analysis.
- Removal or adjustment of outliers was necessary in track_name and artists_name columns for data quality, but it might impact statistical results and patterns identified in the analysis.
- The process involved converting data types to artists_name column can alter the original dataset. However, it enhanced the precision of the findings.


