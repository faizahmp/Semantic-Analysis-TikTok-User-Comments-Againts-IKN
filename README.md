# SEMANTIC ANALYSIS TIKTOK USER COMMENTS AGAINTS IKN (IBU KOTA NUSANTARA)

## Overview

<p align="justify">The relocation of the Indonesian capital city from Jakarta to the North Penajam Paser and Kutai Kartanegara has become a topic that attracted public attention in recent years. One way to find out the response of the related community the transfer of the capital city is through social media. In the context of Capital delivery, TikTok can be an interesting source of information to explore user sentiment on this topic. TikTok user sentiment analysis can provide insight into how the capital transfer plan is set up. 
</p>
<p align="justify">This analysis aims to analyze the sentiments of TikTok users in the comments column regarding transferring videos of the Indonesian capital city and implementing machine learning solutions using natural language processing. Comments will be divided into 2 groups of sentiment: positive and negative. With sentiment analysis, it is hoped that the government can see various points of view from the voices of the people, especially on social media, TikTok.</p>

## Methods

### 01 Data Collection

The comment data collection process uses the [TikTokCommentScraper][link-1] python script and gets 3249 comments from 10 videos. Data is stored in CSV form. There are 3 attributes used: `User@`, `Comment Text`, and `Likes`.

### 02 Data Pre-processing

At this stage we did several pre-processing steps:

- Converting more than one user comments into a list
- Removed @username
- Delete emojis
- Removing punctuation
- Fix words manually
- Removes stopwords
- Tokenization

### 03 Sentiment Analysis

The library used is called [Sensi][link-2] based on Naive Bayes to classify negative and positive comments. This grouping is marked with a value label of 0 for negative comments and 1 for positive comments.

## Results

From a total of 2898 comments analyzed, 1185 comments (41%) indicated positive sentiment, while 1713 comments (59%) indicated negative sentiment. For more details please visit [the details][link-3].

## Team Members

| Name                    | Student ID |
| :---------------------- | ---------: |
| Muhammad Haerul         | H071201033 |
| Muhammad Azhar Tawakkal | H071201041 |
| Faizah Mappanyompa      | H071201045 |

[link-1]: https://github.com/cubernetes/TikTokCommentScraper
[link-2]: https://github.com/GazDuckington/sensi
[link-3]: https://github.com/faizahmp/Semantic-Analysis-TikTok-User-Comments-Againts-IKN/blob/main/(Results)_Semantic_Analysis_TikTok_User_Comments_Againts_IKN.ipynb
