# YouTube Analysis (penguinz0 channel) Project

<p align="center"> Wordcloud on penguinz0 all video's title (view <b>2-Preprocessing and EDA.ipynb</b> notebook)
  
![image](https://github.com/billharit/penguinz0-channel-analysis/assets/77628684/54f1600a-b097-4dc5-9133-3556a7ffb16d)
  
</p>

## Overview

This project is an analysis of a YouTube channel, specifically focusing on [penguinz0](https://www.youtube.com/user/penguinz0). The analysis is performed using Jupyter Notebook, with two main components: data collection and preprocessing/EDA.

1. **1-Collecting Data.ipynb**: This Jupyter Notebook contains the code for collecting data from YouTube, utilizing the Google API. The collected data includes information about the videos, views, comments, likes, and more.

2. **2-Preprocessing and EDA.ipynb**: In this Jupyter Notebook, the collected data is preprocessed and explored through Exploratory Data Analysis (EDA). This step involves data cleaning and data visualization.

## Data Collection

To collect data from YouTube, the Google API is used. You will need to set up your API credentials and provide them in the Jupyter Notebook for data retrieval. Make sure to follow the [Google API documentation](https://developers.google.com/youtube/v3/quickstart/python) for setup instructions.

## EDA and Preprocessing

The preprocessing and EDA steps involve cleaning the collected data and gaining insights into the YouTube channel's performance. I use the Seaborn Python library to analyze the data into interesting-looking plots.

## 'penguinz0' Folder Contents

The 'penguinz0' folder contains essential data files used in this YouTube analysis project. These files are used for analysis and gaining insights into penguinz0's YouTube channel. Following `1-Collecting Data.ipynb` notebook should produce these files.

### `video_ids.pkl`

- **Description**: This file is a serialized list of video IDs related to penguinz0's YouTube channel. Video IDs are unique identifiers for each video, and they are crucial for linking comments and other data back to specific videos.

### `video_df.pkl`

- **Description**: `video_df.pkl` is a Pandas DataFrame containing detailed information about the videos from penguinz0's YouTube channel. The DataFrame includes the following columns:
  - `id`: Video ID
  - `channelTitle`: Title of the channel
  - `title`: Title of the video
  - `description`: Description of the video
  - `tags`: Tags associated with the video
  - `publishedAt`: Date of publication
  - `viewCount`: Number of views
  - `likeCount`: Number of likes
  - `favouriteCount`: Number of favorites
  - `commentCount`: Number of comments
  - `duration`: Duration of the video
  - `definition`: Video quality definition
  - `caption`: Whether the video has captions

This DataFrame serves as the foundation for the analysis, offering insights into video characteristics, viewer engagement, and more.

### `comments.pkl`

- **Description**: `comments.pkl` is another Pandas DataFrame, containing video comments associated with penguinz0's videos. The DataFrame includes the following columns:
  - `video_id`: Video ID (linked to `video_df.pkl`)
  - `comments`: A list of comments associated with the video

This dataset enables sentiment analysis, comment sentiment trends, and deeper engagement analysis with the audience.

## Dependencies

You may need to install the following Python libraries for this project. You can do so using

`pip install -r requirement.txt`

```
google-api-python-client
pandas
matplotlib
isodate
seaborn
wordcloud
nltk
```

## References

```
https://www.youtube.com/watch?v=D56_Cx36oGY&ab_channel=ThuVudataanalytics
https://github.com/thu-vu92/youtube-api-analysis/tree/main
```
