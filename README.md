# real-estate-web-scraper
A webscraper based on the selenium webdriver to scrape data off of indian real-estate websites

## Motivation behind building this web-scraper

My main motivation behind building this webscraper was due to the fact that there is virtually no available dataset for the real estate industry in India. While you can find housing datasets for cities like Boston and San Francisco, there isn't any available data for analysis for cities like New Delhi, Bangalore, Kolkata, you get the gist. While I could have paid a company to get some data for my project, I'm pretty miser about these things so I decided to build a webscraper to get atleast a few basic fields in a nice dataset. 

## Problems

> So webscraper huh, should be easy! 

Well it wasn't! A lot of the main real estate listing websites in India like 99acres.com, commonfloor.com and others have their html structured like a jenga tower after a drinking game...basically you have no idea how it is still standing. I did however, find a website called Sulekha.com, which was pretty neatly organized in terms of it's html and javascript. So I decided to go with it. 

>Well, show me the CODE!

Easy there. You realize once you load the webpage is that it's not a numbered pages layout, where you click on next page, and then again, and then again, conveneniently scraping off of static webpages. Nope, this is a dynamically loaded webpage where you have to scroll down the page for it to load more listings. I realized then that I could be over  my head with this being my first webscraping project, but after a few hours I figured it out. I ended up using the Selenium Webdriver to dynamically load the listings and then shut down once there are no more listings to show. And THEN we can scrape all the listings nested in the HTML div tags!

> ALright, now where do we start?

I'm going to try to list everything that I used in this project, including links on how to install Selenium Webdriver on different operating systems and the libs I used to scrape. Even then, I faced a lot of difficulties scraping data from this website, namely their server not responding after a certain number of requests, the page crashing, some missing listings, etc, etc. The point of this is not to give you a whole end to end solution, but to help anyone out there trying to scrape data from Indian real estate websites! 

I could go on a long rant about how it's almost impossible to make sense of the internal structure of the html of all these websites, and sure that would be appropriate. But we still gotta do what we gotta do, and this code worked for me. I hope it works for you out of the box, and if it doesn't, I hope a few edits here and there make it work for you! Let's start scraping!

### Selenium WebDriver installation
### Libraries used
