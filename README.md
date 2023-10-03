# Mars Web Scraping and Data Analysis Project
Used knowledge of HTML elements and attributes to extract/scrape various types of information from [Mars News](https://static.bc-edx.com/data/web/mars_news/index.html) and [Mars Temperature Data](https://static.bc-edx.com/data/web/mars_facts/temperature.html) sites via automated browsing with Splinter and HTML parsing with Beautiful Soup. 

## Part 1: Scrape Titles and Preview Text from Mars News Articles
1. Used automated browsing to visit the [Mars News Site](https://static.bc-edx.com/data/web/mars_news/index.html) and inspected page to identify which elements to scrape.
2. Created a Beautiful Soup object and used it to extract text elements from the website.
3. Extracted the titles and preview text of the news articles that were scraped. Stored each title-and-preview pair in a Python dictionary and gave each dictionary two keys: title and preview. Stored all dictionaries in a Python list.

## Part 2: Scrape and Analyze Mars Weather Data 
1. Used automated browsing to visit the [Mars Temperature Data Site](https://static.bc-edx.com/data/web/mars_facts/temperature.html). Inspected the page to identify which elements to scrape.
2. Created a Beautiful Soup object and used it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function.
3. Assembled the scraped data into a Pandas DataFrame, using column names with the same headings as the table on the website.
4. Examined the data types that were associated with each column, casting/converting the data to the appropriate datetime, int, or float data types.
5. Analyzed dataset by using Pandas functions to answer the following questions:
    1. How many months exist on Mars?
    2. How many Martian (and not Earth) days worth of data exist in the scraped dataset?
    3. What are the coldest and the warmest months on Mars (at the location of Curiosity)?
    4. Which months have the lowest and the highest atmospheric pressure on Mars?
    5. About how many terrestrial (Earth) days exist in a Martian year?
6. Exported the DataFrame to a CSV file.
