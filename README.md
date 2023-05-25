
Youtube data scrapping and harvesting

Problem Statement:
The problem statement is to create a Streamlit application that allows users to access and analyze data from multiple YouTube channels. The application should have the following features:
  Ability to input a YouTube channel ID and retrieve all the relevant data (Channel name, subscribers, total video count, playlist ID, video ID, likes, dislikes, comments of each video) using Google API.
 Option to store the data in a MongoDB database as a data lake.
 Ability to collect data for up to 10 different YouTube channels and store them in the data lake by clicking a button.
 Option to select a channel name and migrate its data from the data lake to a SQL database as tables.
Ability to search and retrieve data from the SQL database using different search options, including joining tables to get channel details.



## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`Youtube Data APi key`



## Steps to be followed

1. Create the streamlit dashboard :
Using Streamlit library create the dashboard as per the requirement, go through documentation to learn more on streamlit.
https://docs.streamlit.io/library/api-reference/performance/st.cache_data

1. Set up YouTube API access :
Enable the YouTube Data API in Google Developers console and obtain API credentials, go through documentation to learn more on how to extract data using API
https://developers.google.com/youtube/v3/docs

2. Scrape the YouTube data :
Using google-api-python-client library, extract the youtube channel, playlist, videos and comments details.

3. Store the data in MongoDB :
Create the database and collections to Store the extracted data using the pymongo library

4. Migrate the data from MongoDb to SQL :
Based on specific data create the tables, use pymysql library to establish connection with MySQL and migrate the data to tables



