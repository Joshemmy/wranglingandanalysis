## Project Tasks

> The dataset been wrangled is a tweet the tweet archive of a twitter handle @dog_rates. Downloaded through Udacity for this project. The archive contains columns like the tweet_id, timestamp, text.  
> The task for this project would include the various data wrangling processes that would need decisive precision and keen a observation. The quality issues should be at least 8 and the tidiness issues should be at least 2.

> The Data Wrangling Processes includes:
>- Gathering data
>- Assessing data
>- Cleaning data
>- Storing, analyzing, and visualizing our data

## Data Gathering for this Project

> The data in this project was gathered from different sources with variety data gathering methods. For the 3 data sources. 3 methods were used for the data gathering:
>- Importing data via csv
>- Using requests to download data off internet
>- Got data from an API provided by Udacity

## Data Sources
### Enhanced Twitter Archive

>This data was provided by udacity as "twitter-archive-enhanced.csv" which i downloaded. It contained 2356 entries with various columns that I needed to assess and validate if either would be essential for the analysis.

### Image Predictions File

> This data cotains the tweet iamge predictions which is stored in a tsv file as "image_predictions.tsv" which was hosted on Udacity's server. It was downloaded using the Request library through a URL.

### Twitter API Data

> This data is a Json data, which we downloaded from Udacity because I couldn't get my twitter developer account approved. This Json data was stored in "tweet_json.txt". Then we read this file into a pandas Dataframe.

### Data Assessing
> Some quality and tidiness issues were found


| Issue Number | Description | Issue Type |
| --------------- | --------------- | --------------- |
|1| The timestamp entries have "+0000" values added, which is not neccessary. | Quality |
|2| The timestamp column is in string format instead of datetime format | Quality |
|4| There are 181 retweets and 78 tweet replies which was determined by checking the in_reply_to_status_id and retweeted_status_id column | Quality |
|5| There are tweet ratings with rating_denominator columnwith values NOT equal to 10 | Quality |
|6| Invalid dog names | Quality |
|7| There are 59 missing tweets in the expanded_urls column | Quality |
|8| There are only 4 types of sources, and they would be clearer to see if the html codes are removed. | Quality |
|9| Remove entries that have p1_dog, p2_dog, & p3_dog values set to false. These entries are not dogs | Quality |
|10| Convert data type of tweet_id to object string data type for merging | Quality |
|11| The Assessment Key Points indicates that we’re only interested in “original tweets”, no “retweets”; and these tweets are stored retweeted_status_id, retweeted_status_user_id and retweeted_status_timestamp, in_reply_to_status_id and in_reply_to_user_id columns. columns | Tidiness |
|12| There are 4 columns that do not comform to the rules of tidy data. doggo, floofer, pupper, puppo columns should be in one column as they are dog stages. | Tidiness |
|13| The dog breed that was predicted with the highest confidence level can be combined with the df_archive table  | Tidiness |
|14| The df_tweets table should be combined with the archive table. | Tidiness |
|15| The column name id is tweet_id in other tables. Renaming would be neccessary to ensure consistency | Tidiness |

## Cleaning Data
> A lot of effort was put into the cleaning, I sourced for ideas and knowledge all over the internet. My go to sources were https://google.com, https://stackoverflow.com, https://github.com for guidance and proper understanding of the effective ways to take to ensure a resolve of any roadblocks i faced.  I feel I developed a whole lot from this project and would be able to take on other projects that are similar.  Once the cleaning was done. I stored my data then conducted my analysis to produce data driven insights
