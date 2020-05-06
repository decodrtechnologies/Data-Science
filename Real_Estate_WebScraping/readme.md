## Web Scraping Real-Estate



---
## Why Web-Scrape ?
The 70 % time of a Data Scientist goes into collecting and cleaning the Data. Till now we have taken the data from different repositories and used it for our analysis. What if the data that we are looking for is not present in any repositories and we find it on a website. How will you go about collecting the data ? We can either manually copy paste the data or automate the process. If we manually copy and paste the data it will take much time . We can automate this process using web scraping.


---

**Web Scrraping is a technique to scrape the data present of the web.** 


We will be scraping the real estate data from **Makaan.com**  for the 
properties listed for sale in Hyderabad. We will scrape the first 500 pages of the listing. Each page has 20 listing so after scraping the website we should have 10,000 listings records.

Libaries used :
 * Pandas
 * Requests
 * BeautifulSoup
 * Time
 * Random

 Link to the listing - [Apartments in Hyderabad](https://www.makaan.com/hyderabad-residential-property/buy-property-in-hyderabad-city?budget=,&page=1)
 
## Web Scraping Workflow

  <a href="https://imgur.com/2yHeAam"><img src="https://imgur.com/2yHeAam.png" title="source: imgur.com" /></a>
  * Identify Website and it's structure
  * Build a scraper to scrape data from different tags.
  * Store the scrapped data in Structure tables.
  
   
