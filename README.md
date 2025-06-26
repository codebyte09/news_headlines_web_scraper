# news_headlines_web_scraper
This Python script scrapes news headlines from a given URL using requests and BeautifulSoup. It extracts text from common headline tags (&lt;h1>, &lt;h2>, &lt;h3>), saves them to headlines.txt, and then prints the extracted headlines to the console for immediate viewing. Simple, efficient, and great for quick content extraction.
# News Headline Scraper

## Project Description

This Python script is a simple web scraper designed to extract news headlines from a specified website. It uses the `requests` library to fetch the webpage's HTML content and `BeautifulSoup` for efficient parsing to identify and extract headline text. The extracted headlines are then saved into a plain text file (`headlines.txt`), and for immediate review, the content of this file is also printed to the console.

## Features

* **Web Scraping:** Fetches HTML content from a given URL.
* **Headline Extraction:** Parses HTML to find common headline tags (`<h1>`, `<h2>`, `<h3>`).
* **File Output:** Saves extracted headlines to a `headlines.txt` file.
* **Console Display:** Prints the scraped headlines directly to the terminal for quick viewing.

## Requirements

To run this script, you need Python 3 installed, along with the following libraries:

* `requests`: For making HTTP requests to fetch web pages.
* `beautifulsoup4`: For parsing HTML and XML documents.

## Installation

1.  **Clone the repository (or download the script):**
    If you're using Git:
    ```bash
    git clone [https://github.com/YourUsername/your-repo-name.git](https://github.com/YourUsername/your-repo-name.git)
    cd your-repo-name
    ```
    (Replace `YourUsername` and `your-repo-name` with your actual GitHub username and repository name if you upload it there.)

2.  **Install the required Python libraries:**
    ```bash
    pip install requests beautifulsoup4
    ```

## Usage

1.  **Open the script:**
    Open the `news_scraper.py` file in a text editor.

2.  **Set the target URL:**
    Locate the line `news_url = "https://www.bbc.com/news"` and replace `"https://www.bbc.com/news"` with the URL of the news website you wish to scrape.

    **Important Note:** Always check a website's `robots.txt` file (e.g., `https://www.example.com/robots.txt`) and their terms of service before scraping. Some websites prohibit scraping or have specific rules. Be a responsible scraper!

3.  **Run the script:**
    Execute the script from your terminal:
    ```bash
    python news_scraper.py
    ```

## Output

Upon successful execution, the script will:

* Print a confirmation message indicating how many headlines were scraped and saved to `headlines.txt`.
* Then, it will print the entire content of the `headlines.txt` file directly in your terminal.
* A file named `headlines.txt` will be created in the same directory as the script, containing one headline per line.

## Error Handling

The script includes basic error handling for:

* Network issues (e.g., website not found, connection errors).
* Unexpected errors during the scraping or file operations.

If no headlines are found on the page (e.g., due to changes in the website's HTML structure or if the specified tags don't contain headlines), a message will be displayed indicating this.
