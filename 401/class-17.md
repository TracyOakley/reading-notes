# Class 17 Notes - Web Scraping

[Back to Home](../README.md)

### [Web Scrape with Python in 4 minutes](https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460)

+ Web scraping is a technique to automatically access and extract large amounts of information from a website, which can save a huge amount of time and effort.
+ Important notes about web scraping:
  + Read through the website’s Terms and Conditions to understand how you can legally use the data. Most sites prohibit you from using the data for commercial purposes.
  + Make sure you are not downloading data at too rapid a rate because this may break the website. You may potentially be blocked from the site as well.
+ The first thing that we need to do is to figure out where we can locate the links to the files we want to download inside the multiple levels of HTML tags. Simply put, there is a lot of code on a website page and we want to find the relevant pieces of code that contains our data.
+ We start by importing the following libraries.
  + import requests
  + import urllib.request
  + import time
  + from bs4 import BeautifulSoup

### [Web Scraping](https://en.wikipedia.org/wiki/Web_scraping)

## ***[How to scrape websites without getting blocked](https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/)***

### [Track Amazon Prices - Video](https://www.youtube.com/watch?v=Bg9r_yLk7VY)

### [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/)
