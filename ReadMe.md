# Amazon Audible Web Scraping Bot

![alt text](image.png)

## Overview

This is a Selenium-based web scraping bot designed to scrape book information from Amazon Audible. The bot targets the Audible search page and extracts the book title, author, and duration of the books listed.

## Target URL

The target URL for this scraping task is: [https://www.audible.com/search](https://www.audible.com/search)

## Libraries Used

- `selenium`: For automating web browser interaction.
- `pandas`: For data manipulation and storage.

## Instructions
-   **Install the required libraries:**
    ```shell
    pip install selenium pandas
    ```
-   **Download the Chrome WebDriver:**<br>
    Ensure you have the Chrome WebDriver installed and it's compatible with your Chrome browser version. Download ChromeDriver.

-   **Run the Script:**
    ```Python
    cd ./code
    python aa_scrap.code.py             #runnign the main scraing script
    python aa_scrap_headless.py         #running in headless mode
    python aa_scrap_page_wait.py        #running with implicit and explicit waits
    python aa_scrap_pagination.py       #running the pagination script
    ```
-   **Check the Output**<br>
    All the scrapped data is stored inside `data_dd` directory

## Notes
-   The script uses **XPath** to locate elements on the page.
-   The Chrome WebDriver will start and navigate to the Audible search page, maximize the browser window, and scrape the required data.
-   Ensure that the structure of the Audible website has not changed as it may affect the XPath queries used in the script.
