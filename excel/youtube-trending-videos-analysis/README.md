# YouTube Trending Analysis

## Overview
This project analyzes a dataset of YouTube videos that appeared on the daily trending list to identify patterns associated with video views and trending performance.

The analysis explores video characteristics, engagement metrics, categories, and view counts to understand what distinguishes high-performing trending videos. The project also considers additional data that could be collected to better explain why some videos receive substantially more views than others.

The project was completed in Excel as part of the Global Career Accelerator Data Analytics program.

## Business Question
What factors are associated with higher view counts among trending YouTube videos, and how can content creators use these insights to improve their content strategy?

## Data
The dataset contains **6,351 trending video records** and includes information about each video's content, category, publication date, views, and engagement.

Key variables include:
- Video ID
- Trending date
- Publish time
- Video title
- Channel
- Category
- Tags
- Views
- Likes
- Dislikes
- Comments
- Comments disabled
- Ratings disabled
- Video error or removed

The dataset contains **7 numeric columns, 5 text columns, and 3 Boolean columns**.

Some numeric-looking fields require special treatment. For example, `trending_date`, `publish_time`, and `category_id` should not be treated as standard numerical measures for calculations such as averages or sums.

## Analysis

### 1. Understanding the Dataset
I first examined the structure and data types of the dataset using the provided data dictionary.

This included identifying:
- Numeric variables
- Text variables
- Boolean variables
- Variables that should not be treated as standard numerical measures
- The meaning of individual fields

Understanding the structure of the dataset helped determine which variables could be used for quantitative analysis and which required categorical or date-based interpretation.

### 2. Exploring Key Metrics
I used Excel functions and filtering to answer questions about the dataset, including:
- Number of videos in the dataset
- Total likes across trending videos
- Average views per trending video
- Number of videos published before 2010
- Highest-viewed video outside the Music and Entertainment categories
- Number of Gaming videos with more than 10 million views
- Number of Nonprofits & Activism videos with above-average views

### 3. Category Analysis
I compared video performance across different YouTube categories.

The analysis showed that view counts vary substantially between categories. This is important when evaluating whether a particular number of views should be considered exceptional.

For example, a fixed threshold such as 2 million views can represent very different levels of performance depending on the category.

### 4. Defining Exceptional Videos
I examined the distribution of views among trending videos and considered whether a video with 2 million views should automatically be classified as exceptional.

The distribution of views is heavily skewed, with most videos receiving fewer than 2 million views.

However, category differences make a fixed view threshold less useful for defining exceptional performance.

A more useful approach would be to compare a video's views with other videos in the same category and with a similar age since publication. Percentiles could be used to identify videos that significantly outperform comparable videos.

### 5. Factors Associated With Trending Performance
Based on the analysis, two important factors identified were:
- **Video category**
- **Audience engagement**

The analysis also suggests that factors such as topic relevance, title, and the timing of publication may influence a video's ability to reach a larger audience.

These factors should be treated as potential influences rather than established causal relationships because the dataset does not contain enough information to isolate their individual effects.

## Key Findings
- The dataset contains **6,351 trending video records**.
- View counts are heavily skewed, with most trending videos receiving relatively fewer views than the highest-performing videos.
- A video with **2 million views is generally noteworthy and above average**, but whether it is exceptional depends on its category and other characteristics.
- Category differences are important when comparing view counts. A view count that is exceptional in one category may be closer to average in another.
- Music, Entertainment, Film & Animation, and Gaming are examples of categories identified in the analysis as having relatively high view counts.
- The analysis identified **5 Gaming videos with more than 10 million views**.
- The analysis identified **2 Nonprofits & Activism videos with more views than the overall average**.
- The video **"To Our Daughter"** had the highest view count among videos outside the Music and Entertainment categories in the analyzed dataset.

## Content Strategy Recommendations
Based on the analysis, a content strategy could focus on increasing both reach and audience engagement.

Potential strategies include:
- Create compelling and relevant video titles.
- Encourage viewers to like and comment.
- Connect content to timely topics and subjects that audiences are already searching for.
- Consider categories and topics with broader audience appeal.
- For niche subjects, package content in a way that makes it accessible to a broader audience.
- Publish consistently to increase opportunities for high-performing videos.

These recommendations should be viewed as strategic considerations rather than proven causal effects because the available dataset does not contain all of the variables needed to establish why individual videos became successful.

## Additional Data for Future Analysis
The analysis identified several additional variables that could provide a better understanding of what drives video views.

### Channel Size
The number of channel subscribers could help determine whether established channels have an advantage because they begin with a larger potential audience.

### Engagement
Additional engagement metrics such as shares, likes, comments, and engagement rates could help identify relationships between audience interaction and video performance.

### Watch Time and Audience Retention
Average watch duration, percentage of the video watched, and audience retention could provide information about whether videos that hold viewers' attention tend to receive more views.

### Video Length
Comparing video length with views and engagement could help identify whether different categories have different patterns of successful video length.

### Upload Timing
Additional information about the day of the week, time of day, month, and season of publication could help identify potential relationships between publishing time and initial performance.

### Titles and Thumbnails
Title length, keywords, and thumbnail characteristics could be analyzed to identify characteristics associated with higher-performing videos.

## Excel Techniques Used
- Excel functions
- Filtering
- Sorting
- Data aggregation
- Category analysis
- Conditional analysis
- Data interpretation
- Exploratory data analysis
- Business-focused recommendations

## Project Context
This project was completed as part of the Global Career Accelerator Data Analytics program.

The project simulated a data analyst scenario involving YouTube trending videos. The analysis focused on understanding the structure of a large dataset, exploring key performance metrics, identifying patterns across categories, and translating findings into recommendations for improving content strategy.
