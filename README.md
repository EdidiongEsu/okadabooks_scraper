# okadabooks_scraper
  This scraper is used to remove details from all available bookcards in the website https://okadabooks.com. Okadabooks is an online store for african literature based in Nigeria.
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
  
 Selenium is used in this project because automation is required. There are 22 categories in the website and in each category there is a LoadMore button. When the loadMore button is tapped on by a user, it reveals more content. To be able to get all bookcards from the website, The load more button must be pressed till it is no longer available. The crawling algorithm must imitate user interaction in order to avoid being blocked and to also make sure too many requests are not sent to the website at once. The extracted data set will be stored in this repository. The data extracted will be used for some EDA which will be posted in this repository.
 
 **LoadMore Button**
  
  ![](https://github.com/EdidiongEsu/okadabooks_scraper/blob/master/okadabooks_pictures/load_more%20button.PNG)
  
  There are different types of pagination which include infinite scrolling (common in Twitter), serial pagination and a lot more. In this project, LoadMore pagination is used where a tap triggers more content. Here Javascript is used, that why beautiful soup used alone won't work. Action class click in selenium helps to scroll down to the end of the webpage after webelement click has been used. I hope you have some fun with the code.
 
 ***Happy coding!!!***
