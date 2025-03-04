
# Web Scraping Project for Real Estate Contractors

This project is a web scraper built using Python to collect information about real estate contractors and agents from multiple sources, including the BBB and Realtor.com. The scraper is built in an **IPython notebook** and is designed to run efficiently while preventing being blocked by the server. The data collected is then processed and saved as CSV files for further analysis.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Data Processing](#data-processing)
6. [Scheduler](#scheduler)
7. [Requirements](#requirements)
8. [Conclusions](#Conclusions)
9. [Contact](#Contacts)

---

## Project Overview

This project scrapes data from:
- **BBB (Better Business Bureau)**: Collects contractor information like name, company, industry, contact, and location.
- **Realtor.com**: Collects real estate agent data, such as name, agency, experience, and GCI (Gross Commission Income).

The project also includes:
- Pagination support to scrape multiple pages of data.
- Data cleaning and processing with Pandas.
- Synthetic ratings based on the GCI data.
- An automated scheduler to run the scraper periodically.

---

## Features
- **Real Estate Contractors**: Gathers data on contractors, including name, company, industry, contact details, and location.
- **Real Estate Agents**: Extracts agent names, agency, experience, and GCI data.
- **Data Cleaning**: Cleans and processes data (e.g., converting GCI to numeric values, handling missing data).
- **Scheduler**: Runs the scraper every 6 hours using **APScheduler** to keep the data fresh.
- **Output**: Data is saved in CSV format for easy use.

---

## Usage

To run the web scraping process manually, open the IPython notebook (`.ipynb`) and run the cells in sequence. Here's a quick overview of how to use the project:

### 1. Scraping BBB Data

This section scrapes contractor data from the BBB website and stores it in a CSV file.

### 2. Scraping Realtor.com Data

This section scrapes real estate agents' data from Realtor.com and saves the information in a CSV file.

### 3. Data Processing

After scraping, the data is processed:
- GCI values are converted into numeric values.
- Synthetic ratings are generated based on the GCI range.
- The data is cleaned (removal of duplicates and irrelevant entries).

### 4. Scheduled Scraping

The scraper can also be scheduled to run periodically. The `APScheduler` will run the scraper every 6 hours to keep your data fresh.

---

## Requirements

You can install the necessary dependencies by using the provided `requirements.txt` file.

```txt
cloudscraper==1.2.55
beautifulsoup4==4.11.1
pandas==1.3.5
numpy==1.21.2
apscheduler==3.8.1
ipykernel==6.6.1
```


## Conclusion

This project provides a reliable and efficient way to scrape contractor and agent information from multiple websites, clean the data, and store it in an easily accessible format. The integration of a scheduler ensures that the data is updated regularly, making it a valuable tool for anyone looking to gather real estate data.

## Contact

For any questions or support, feel free to reach out!

Author: Saad Naveed

Email: [saad.naveed.dev@gmail.com]

GitHub: saadnaveeddev
