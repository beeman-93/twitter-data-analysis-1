# twitter-data-analysis-1
 # Step 1: Get twitter data using snscrape and translate the result using googletrans

 Search term (コロナ　ストレス)　in English (corona stress)

 Language Japanese

 Time period from 2022-07-18 00:00:00 to 2022-07-24 23:59:59

 Remove all tweets with links and retweets

 Links mean urls or any media including images or videos

 Search for the last 100 tweets posted contained search words backtracking from 2022-07-24 23:59:59

# Update about removing links 

Because media (for example, a picture) is also counted as a link. 

If we remove all tweet with links then we are filtering out a lot of data. 

So we need to find a way to keep tweets with links but use data manupulation to remove http(s) links by ourselves. 

# Update about choosing the time period 

Just realized that if we use the defult advanced search on Twitter, the time will return in UTC (Universal Time Coordinated). 
To convert the time to JST (Japan Standard Time), simply using the following line of code: 

until:2022-07-25_00:00:00_JST since:2022-07-18_00:00:00_JST

# Update about getting tweets with 2 sets of search terms 

Simply adding one "OR" clause helps to get 2 sets of search terms
