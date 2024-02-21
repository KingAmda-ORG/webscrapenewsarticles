# Google News Top Stories Scraper

This Python script scrapes the top stories from Google News and outputs a list of articles with their titles and links.

## Requirements

- Python  3.x
- `requests-html` library

## Installation

Install the required `requests-html` library using pip:

bash pip install requests-html

## Usage

Run the script with Python:
`bash python news_scraper.py`


## How It Works

1. **Importing Libraries**: The script imports the `HTMLSession` class from the `requests-html` library, which is used to make HTTP requests and render JavaScript.

2. **Creating a Session**: An instance of `HTMLSession` is created to manage the requests to the website.

3. **Fetching the Page**: The script makes a GET request to the Google News top stories page URL.

4. **Rendering the Page**: The HTML content of the page is rendered using the `render` method, which executes JavaScript and loads dynamic content.

5. **Finding Articles**: The script searches for all `article` elements on the page, which typically contain the news articles.

6. **Extracting Article Information**: For each `article` element, the script finds the first `h3` element, which usually contains the title of the article. It extracts the text of this element as the title and any associated links as the link.

7. **Storing Article Information**: The script creates a dictionary with the title and link of each article and appends it to a list.

8. **Output**: The script prints the length of the list of scraped articles, indicating how many articles were successfully extracted.

## Note

- This script is designed to scrape the top stories from Google News for the UK region (`en-GB`) and language (`GB:en`).
- The script uses a `try`/`except` block to handle cases where certain `article` elements may not have the expected `h3` elements, preventing the script from crashing due to exceptions.
- The `scrolldown` parameter in the `render` method is set to `5` to simulate scrolling down the page, which can help load more content if the website uses infinite scrolling.
- The script does not handle pagination, so it only scrapes the first page of top stories.

## Disclaimer

Web scraping should be performed in accordance with the terms of service of the website being scraped. Google News' terms of service may prohibit scraping. This script is provided for educational purposes and should not be used for unauthorized web scraping.
# Google News Top Stories Scraper

This Python script scrapes the top stories from Google News and outputs a list of articles with their titles and links.

## Requirements

- Python  3.x
- `requests-html` library

## Installation

Install the required `requests-html` library using pip:

bash pip install requests-html

## Usage

Run the script with Python:
`bash python news_scraper.py`


## How It Works

1. **Importing Libraries**: The script imports the `HTMLSession` class from the `requests-html` library, which is used to make HTTP requests and render JavaScript.

2. **Creating a Session**: An instance of `HTMLSession` is created to manage the requests to the website.

3. **Fetching the Page**: The script makes a GET request to the Google News top stories page URL.

4. **Rendering the Page**: The HTML content of the page is rendered using the `render` method, which executes JavaScript and loads dynamic content.

5. **Finding Articles**: The script searches for all `article` elements on the page, which typically contain the news articles.

6. **Extracting Article Information**: For each `article` element, the script finds the first `h3` element, which usually contains the title of the article. It extracts the text of this element as the title and any associated links as the link.

7. **Storing Article Information**: The script creates a dictionary with the title and link of each article and appends it to a list.

8. **Output**: The script prints the length of the list of scraped articles, indicating how many articles were successfully extracted.

## Note

- This script is designed to scrape the top stories from Google News for the UK region (`en-GB`) and language (`GB:en`).
- The script uses a `try`/`except` block to handle cases where certain `article` elements may not have the expected `h3` elements, preventing the script from crashing due to exceptions.
- The `scrolldown` parameter in the `render` method is set to `5` to simulate scrolling down the page, which can help load more content if the website uses infinite scrolling.
- The script does not handle pagination, so it only scrapes the first page of top stories.

## Disclaimer

Web scraping should be performed in accordance with the terms of service of the website being scraped. Google News' terms of service may prohibit scraping. This script is provided for educational purposes and should not be used for unauthorized web scraping.
