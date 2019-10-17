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
  
 Selenium is used in this project because automation is required. There are 22 categories in the website and in each category there is a LoadMore button. When the loadMore button is tapped on by a user, it reveals more content. To be able to get all bookcards from the website, The load more button must be pressed till it is no longer available. The crawling algorithm must imitate user interaction. The extracted data set will be stored in this repository.
 
 Happy coding!!!
