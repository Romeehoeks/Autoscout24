# Autoscout24

**Data context: The future of electric cars and the downfall of gas cars**

Scope: Electric and gas cars in The Netherlands (with the abilaty to progress into The Benelux)

*Motivation*
Buying a car is a quite time-consuming investment, buyers stay around 3 months in the market before purchasing their car (Cox Automotive, 2018). According to research in the United States 95% of the people that bought a car, used a digital source of information to find their car (Schueller, 2017). Autoscout – of German descent –  helps people find their car and is the biggest online car market in Europe with more than 2 million cars on their website.

*_Why Autscout?_*

Autoscout24 is very organized and brings together consumers and dealers. We have chosen this source for several reasons. The first one is that this website is showing the exact price of the car, it does not allow bidding and does not show lease prices (which are monthly). Next to that Autoscout24 has both the option to filter per country and range. Filtering by country makes it is easy to extract only the data for cars in the Netherlands, but if we would like to expand our database in the future and scrape cars from Belgium and Germany as well, it is easily possible by changing a filter. Also, autoscout24 has a great offer that allows both private sellers and businesses to sell cars. Furthermore, it is possible to extract all the needed data from the search page, so there is no need to scrape the personal page of a car as well. Which makes it very practical to scrape. 

The purpose of our database is to provide consumers with information so that they can compare electric cars with gasoline cars. This can be useful if a consumer for example is in doubt about buying an electric car or a gasoline car. Within the database, it is possible to filter on the following variables: price, km, year, PK, brand, type, dealership, and attributes. Which makes it possible to make for example comparisons between the value/ km ratio of electric and gasoline cars.

To run the Scraper, Jupyter Notebook and Python is required:

We have used BeautifulSoup to scrape raw text and features from the Autoscout24 website. All the infor-mation that was needed for making an interesting and complete database was directly observable on the website. There was not any additional data required. To gather all the URLs, we have for-looped through multiple filters (the reason why is explained in 2.2). We then requested each URL with BeautifulSoup and used the soup.find().text to locate and withdraw the information. This process was completed within the listings page and for each detailed product page. At last, we used a combination of the CSV package and pandas package to save all the information into a file. To make the web scraper Python code was used. To set up this web scraper we used the software program Jupyter Notebook. This program makes writing Py-thon code more accessible and helps with visualizing and controlling the process. The website of Au-toscout24 has an API available, but this is only for sellers and did not give us enough access and infor-mation to complete the database. Therefore, web scraping was the best option. We choose for Beautiful-Soup because of the ease to use and their comprehen-sive documentation. Also other packages  were used such as, requests, time, datetime, csv, json and pan-das to finalize the Python code.  
