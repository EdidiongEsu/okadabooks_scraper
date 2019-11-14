# okadabooks_scraper
  This scraper is used to remove details from all available bookcards (a summary of each book) in the website https://okadabooks.com. Okadabooks is a popular online store for african literature based in Nigeria. Since the company was founded in 2013, it has helped increase the reading culture in the country and pioneered a lot of writing initiatives. For more info, check the [website](https://okadabooks.com.). 
  Here is what one of the bookcards look like. Highlighted are some of the details that will be scrapped in this project.

   ![](https://github.com/EdidiongEsu/okadabooks_scraper/blob/master/okadabooks_pictures/Capture.PNG)
            
**Full list of what will be scraped are:**

  **1**)Title
  
  **2**)Author
  
  **3**)Genre
  
  **4**)Price
  
  **5**)Reads
  
  **6**)Ratings
  
  **7**)Blurb (the description)
  
  **8**)Booklink
  
  ## Dynamic content
When any kind of interaction with the webpage is required during webscraping, it is no longer a static one but becomes a dynamic one. Here, selenium comes to the rescue. Selenium is used in this project because automation is required. There are 22 categories in the website and in each category there is a LoadMore button. When the loadMore button is tapped on by a user, it reveals more content. To be able to get all bookcards from the website, The load more button must be pressed till it is no longer available. The crawling algorithm must imitate user interaction in order to avoid being blocked and to also make sure too many requests are not sent to the website at once. The extracted data set will be stored in this repository. The data extracted will be used for some EDA which will be posted in this repository.
    
 
 **LoadMore Button**
 Before scrapping:
  
  ![](https://github.com/EdidiongEsu/okadabooks_scraper/blob/master/okadabooks_pictures/loadmore_before_webscraping.PNG)
  
  There are different types of pagination which include infinite scrolling (common in Twitter), serial pagination and a lot more. In this project, LoadMore pagination is used where a tap triggers more content. Here Javascript is used, that why beautifulSoup library used alone won't work. Action class click in selenium helps to scroll down to the end of the webpage after webelement click has been used. In the simplest terms, The idea is for an automated software (in this case chrome driver) to tap the loadmore button in a span of set time till it no longer exists.
  
  **Snapshot of dataframe**
  
  After scraping, cleaning and getting rid of all duplicates in the bookcards gotten, about 18,000 books were left. This excluded books that had been taken down by the aadmin/author after publication. A similarity metric will be calculated with the millions of words in the blurb column and some EDA will be done to understand the reading pattern of Nigerians and at the same time ascertain the influence of the bookstore in this pattern.
  
Here, is what the final table looks like:

![](https://github.com/EdidiongEsu/okadabooks_scraper/blob/master/okadabooks_pictures/dataframe%20table.PNG)

For more experimental data analysis on the data gotten, please check my repository.

 
 ***Happy coding!!!***
