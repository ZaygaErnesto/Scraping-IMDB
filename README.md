# IMDb Top 250 Movies Web Scraper
This project is a simple Python script that scrapes the Top 250 Movies from IMDb using Selenium and BeautifulSoup.
The script collects:
- Movie title
- Release year
- IMDb rating
- Movie detail URL
- Movie synopsis
## Features
- Scrapes IMDb's Top 250 movies.
- Retrieves detailed information including movie synopses.
- Uses a custom user-agent to minimize bot detection.
- Stores the scraped data in a Pandas DataFrame.
## Requirements
- Python 3.7+
- Google Chrome
- ChromeDriver (compatible with your Chrome version)
## Installation
1. Clone this repository:
```
git clone https://github.com/ZaygaErnesto/Scraping-IMDB.git
cd Scraping-IMDB
```
2. Install the required Python packages:
```
pip install selenium beautifulsoup4 pandas
```
## Usage
1. Ensure that ChromeDriver is either added to your system's PATH or located in the same directory as the script.
2. Run the script:
```
python Web-Scraping.py
```
3. The output will be displayed in the terminal, showing the title, release year, rating, and synopsis for the top 5 movies by default.
## Code Structure
- setup_driver(): Sets up the Selenium WebDriver with a custom user-agent.
- get_top_movies_with_synopsis(driver, jumlah=5): Scrapes movie data and synopses from IMDb.
- main(): Main function that orchestrates the scraping process.
## Notes
- By default, the script fetches 5 top movies. You can change the jumlah parameter in get_top_movies_with_synopsis() to fetch more or fewer movies.
- A stable internet connection is recommended to avoid scraping errors.
- Important: IMDb's HTML structure (especially class names used for elements) may change over time.
If the script fails to locate elements, please check and update the CSS selectors by inspecting the latest IMDb page manually.
