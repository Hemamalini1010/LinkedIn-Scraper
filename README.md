# LinkedIn-Scraper
Find the openings for Data Analyst Role and generate Tableau report

Problem Statement:
Scraping the Linkedin browser to fetch all the openings for Data Analyst Role and generate the trend for current date. 
-To understand the Job Market and opportunities 
-To check the companywise openings

Note: URL has 2 constantly changing variable, 1) Page number  2) Start (This range from 0 to 100 , and increased as 25)

Tableau Dashboard Link - https://dub01.online.tableau.com/#/site/kirubakaranjayakumar/views/linkedinjobs-trendanalysis/JobMarketTrend?:iid=4

Tools Used - Jupyter , Tableau

Code - Walkthrough
----------------------
1) Import essential libraries
2) Open Csv File with headers
3) Read the URL
4) Create funtion 
    > Assign variables 
    > Read the tags & extract class
    > Since Time tag has different attribute for current date and others, Current date fetched as NONE. So introduced if class to handle this logic
    > Loops have been introduced to handle URL variable - Start(here i mentioned as Page_number)
 5) Loop the function for number of pages(Here i have seen 4K jobs in search, so introduced the range(0,3) ) - Change it based on your search criteria
