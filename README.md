# car-sale-scraping
A simple tool to scrape images, pricing and information of available 2nd-hand cars and receive email notification on desired car types. 

### Usage
Hong Kong's most active platforms for buying and selling used cars are mostly available in Chinese and difficult to assess for foreigners. To help expats in Hong Kong browse available used cars at ease and receive the most up-to-date market information, I developed a web scraper to collect images and basic information of desired car types; users can specify brands, years, model types, etc. The information, in turn, is collected in a concise table format and sent to users via automated email notifications.

Althought not currently developed, the scraper can also be deployed in a web application (e.g. Streamlit) instead of email notifications for more active and hands-on searches.

### Workflow
PART I: Scraping
I've used a combination of Beautifulsoup and Selenium. As the code is specific to certain website formats, please reach out for customization.

PART II: Visualization & Storage
Information scraped and stored include: 'ID','model','seats','size','year','price','image','URL'. 
This is in turn displayed on a HTML page and stored as a csv file.

PART III: Email Notification
The HTML and CSV file above are in turn sent to users via automated emails periodically. 

### Potential further usage
This tool is currently used for simple information scraping/displaying/storing purpose. By augmenting additional dimensions, such as time, the same tool can be enhanced to analyze market trends, predict pricing and spot mismatches in the 2nd-hand car market.
