#Twitter Scraper:
The problem statement is to Scrape the data like (date, id, url, tweet content, user,reply count, retweet count,language, source, like count etc) from twitter.

Approach:
By using the “snscrape” Library, Scrape the twitter data from Twitter.For importing 'snscrape' library snscrape needs to be installed using !pip install snscrape.
To run git cli commands, you have to have git installed before running your pip command by using 'pip3 install git+https://github.com/JustAnotherArchivist/snscrape.git'.
To scraping tweet data from twitter - Import libraries and packages named:import snscrape.modules.twitter as sntwitter & import pandas.
Create a dataframe with date, id, url, tweet content, user,reply count, retweet count,language, source, like count.
Store each collection of data into a document into Mongodb along with the hashtag or key word we use to  Scrape from twitter. 
eg:({“Scraped Word”            : “****”,
        “Scraped Date”             :dd-mm-yyyy,
        “Scraped Data”             : [{1000  Scraped data from past 100 days }]})
Scrape data and append tweets to list by using TwitterSearchScraper.Create a dataframe from the tweets list using 'DataFrame'.
Import pymongo and from that import MongoClient for database conecgtion establishment.
Once conection setup done and switch to demoCollection and create the document as per mentioned example.
Once all documents created will be inserted by using collection.insert() and print the result.

Create a GUI using 'import streamlit as st' and upload the data into database and download the data into csv and json format.

Results: Able to scrape the twitter data and store that in the database and able to download the data with CSV and JSON formats.
