# Data Science Practice
___
This repo holds projects I did to help me practice data analysis, data scraping, etc. These are projects I did along 
with studying from IBM data science course to teach and polish skills related to the subject.

### Anime Database Analysis
I was curious on possible variables that are correlated with a higher popularity score in an anime. This information 
could be useful in predicting what attributes of an anime can help determine its popularity. After I found open-source
datasets online related to my research I downloaded them and imported them to a postgreSQL database. I extracted 
information I needed using postgreSQL queries. 
##### Correlations studied
* Rating
* Number of episodes 
* Length of the anime in seconds
* Season it released
##### Results
None of the variables tested had a significant correlation with the popularity of the anime. The strongest correlation
found was "Length of the anime in seconds" with an r coefficient of 0.6501514248925572. The number of episodes however
had an r coefficient of -0.26330268930905276. Even though the correlation is not significant the number of episodes have
a negative relation compared to length in seconds with a positive correlation. This suggests that the viewer more likely
to enjoy a series if the episodes length are longer. 

I could not find the r coefficient for Rating and Season are not numeric but the popularity score seem close together
with no about or significant change.

### Books Scrapped Analysis
This project was to practice web scrapping using BeautifulSoup. The website I practiced on is 
https://books.toscrape.com/ which is a site to help practice extracting data from the web. I acquired the skills used in 
this project from the IBM course and a course from udemy called "The Ultimate Web Scraping With Python Bootcamp 2023".
##### What I learned and practiced
I explored different pages of the website extracting information as in book title, rating of it, and price. After data 
was collect and processed it was then saved as a pandas data frame. With the data ready to be handled I wanted to test
te correlation between the length of the title of the book with its rating. It resulted in an R coefficient of 
-0.3273372802263818 stating the two values are not co related.

### Stock Analysis
In this project I gather information on tesla stocks (TLSA) and game stop stocks (GME). I gather history of the stock past 
worth using the yfiance python module and used the Ticker class then the history() method on the instance to do so. I also 
parsed a website using BeautifulSoup module to extract data on the revenue of the stocks by extracting the table with the data
 from the website. The websites I got the data from was [Tesla](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/revenue.htm) and [Game Stop](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/stock.html).
 ##### Purpose
 I was able to display the data in a graph to see if the trend of the stock values and determine if it will be a safe investment to 
 buy some tesla or game stop stocks
 
