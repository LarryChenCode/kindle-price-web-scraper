# kindle-price-web-scraper

# Web Scraping Amazon Kindle Prices

![Web Scraping Project Banner](images/web-scraping.gif)

In this project, I demonstrate how to perform web scraping on Amazon to track the price of Kindle books. This task is accomplished using a variety of Python libraries to efficiently fetch data, parse HTML, and automate the monitoring process.

## Tools Used

The project leverages the following Python libraries:

- `BeautifulSoup` from `bs4` for parsing HTML and extracting the necessary data.
- `requests` for making HTTP requests to Amazon's website.
- `time` and `datetime` for handling timing and scheduling of the price checks.
- `smtplib` for sending email notifications.
- `csv` for reading from and writing to CSV files, facilitating data storage.
- `pandas` as an additional tool for data manipulation and analysis.

## Functionality

The core functionality of this project is encapsulated in a function designed to check the price of a specified Kindle book on Amazon periodically. If the price drops to or below a target price set by the user, the function automatically triggers an email notification to alert the user of this price change.

### How It Works

1. The specified book's URL is used to make a request to Amazon's website.
2. The page's HTML content is fetched and parsed using BeautifulSoup to extract the book's current price.
3. The extracted price is compared against the user's target price.
4. If the book's price is less than or equal to the target price, an email notification is sent to the user, alerting them of the price drop.
5. This process is scheduled to run at regular intervals using the `time` and `datetime` libraries, ensuring continuous monitoring.

## Disclaimer

This project is inspired by [Alex The Analyst](https://www.youtube.com/@AlexTheAnalyst), and is intended for educational purposes only. Web scraping can violate the terms of service of some websites. Always ensure you are in compliance with the legalities and ethical considerations of web scraping for your use case.
