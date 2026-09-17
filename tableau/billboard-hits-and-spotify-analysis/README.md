# Billboard Hits & Spotify Analysis

## Overview
This project analyzes music trends from 1999–2019 by combining Billboard Hot 100 chart data with Spotify audio feature data. The analysis explores changes in genre presence over time and examines relationships between different musical characteristics.

The project was completed in Tableau as part of the Global Career Accelerator Data Analytics program.

## Business Question
How have music genre preferences changed over time, and what relationships exist between the audio characteristics of popular songs?

## Data
The analysis combines two datasets covering music from 1999–2019:
- Billboard Hot 100: Weekly chart rankings, peak position, weeks on chart, artist, song, date, and genre.
- Spotify Song Attributes: Audio characteristics including danceability, energy, acousticness, instrumentalness, liveness, speechiness, tempo, valence, and popularity.

The datasets were combined to connect Billboard chart performance with Spotify audio characteristics.

## Analysis
I created interactive Tableau visualizations to examine genre trends and relationships between song characteristics.

Key analysis included:
- Tracking the proportion of Pop and Rock songs appearing in the Billboard Top 100 over time
- Comparing genre presence between the 2000s and 2010s
- Creating a parameter-driven visualization to explore the presence of eight different genres
- Using Tableau parameters to dynamically select different Spotify audio features
- Comparing audio features such as Valence and Danceability
- Creating calculated fields to classify songs by genre
- Calculating genre proportions within the Billboard Top 100
- Combining Billboard chart information with Spotify audio attributes

## Key Findings
### Pop and Rock Trends
- The proportion of Pop songs in the Billboard Top 100 saw a sharp decrease during 2001–2002, followed by a general resurgence over the remainder of the dataset.
- Rock presence increased from approximately 2000–2002, remained relatively stable from 2002–2013, and then steadily declined through 2019.
- The changing presence of these genres may reflect the growing influence of other genres, changes in music culture, and the emergence of digital music and streaming.

### Genre Growth
Several genres showed a general increase in their presence in the Billboard Top 100 when comparing the 2000s with the 2010s:
| Genre | 2000s | 2010s |
| -------- | -------- | -------- |
| Alternative | 8.44% | 12.12% |
| Dance | 4.80% | 13.13% |
| Electro | 1.11% | 10.10% |
| Rap | 19.19% | 41.41% |

Rap experienced the largest increase among these genres, more than doubling its presence in the Top 100.

### Audio Features
The interactive audio-feature visualization showed a moderate positive relationship between Valence and Danceability. Songs with higher valence generally tended to have higher danceability, although the distribution of songs was sufficiently spread out that the relationship was not particularly strong.

## Visualizations
- [Rock and Pop Popularity](images/rock-and-pop-popularity.png)

- [Proportion of Billboard 100 Songs with Alternative (1999-2019)](images/proportion-of-billboard-100-songs-with-alternative.png)

- [Audio Features - Valence vs Danceability](images/audio-features-valence-vs-danceability.png)

## Interactive Dashboard
[View the interactive dashboard on Tableau Public](https://public.tableau.com/views/BillboardHitsSpotifyAnalysis_17890936457910/WriteAnswersHere?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Tools & Skills
- Tableau
- Data visualization
- Interactive visualizations
- Parameters
- Calculated fields
- Data blending
- Genre analysis
- Time-series analysis
- Comparative analysis
- Audio feature analysis
- Data-driven insights

## Project Context
This project was completed as part of the Global Career Accelerator Data Analytics program and focused on analyzing music industry data to identify trends in genre popularity and relationships between characteristics of popular songs.
