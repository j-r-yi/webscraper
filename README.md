# Web Scraper Learning Project

**DISCLAIMER: This is ONLY A LEARNING PROJECT. The code in this repository is meant for educational purposes only. The author is not responsible for how others use this code. Please adhere to the terms of service and legal guidelines of the websites being scraped.**

---

## Overview
This repository contains two Python scripts demonstrating web scraping techniques for educational purposes. The projects focus on extracting data from web pages, processing it into structured formats like CSV and Excel, and optionally integrating it into a database. Below is a detailed description of each script:

---

### 1. Billboard Hot 100 Scraper
This script extracts data from the [Billboard Hot 100](https://www.billboard.com/charts/hot-100/) chart, including rankings, song titles, authors, album covers, and chart statistics.

#### **Features:**
- Scrapes the top 100 songs along with their rankings, authors, and album cover URLs.
- Extracts chart metadata, such as the date of the chart.
- Parses statistics like last week's position, peak position, and weeks on the chart.
- Exports the scraped data to both CSV and Excel formats for further analysis.

#### **Technologies Used:**
- `requests` for sending HTTP requests.
- `BeautifulSoup` (from `bs4`) for parsing and extracting HTML content.
- `pandas` for organizing and exporting data.

---

### 2. Hardware World Engine Oil Scraper
This script logs into the [Hardware World](https://www.hardwareworld.com/) website, navigates to the Automotive Engine Oil section, and scrapes product details like model numbers, names, and prices.

#### **Features:**
- Automates login to the website using Selenium.
- Navigates through website links to the target product category.
- Scrapes product details (model number, product name, price) from the webpage.
- Exports the extracted data to both CSV and Excel files.
- Optionally saves the data into a MySQL database.

#### **Technologies Used:**
- `Selenium` for browser automation and web scraping.
- `pandas` for organizing and exporting data.
- `SQLAlchemy` for integrating the scraped data into a MySQL database.

---

## Prerequisites
### Libraries and Tools:
Both scripts require Python 3.x and the following libraries:
- **For Billboard Hot 100 Scraper**:
  - `requests`
  - `BeautifulSoup`
  - `pandas`
- **For Hardware World Engine Oil Scraper**:
  - `selenium`
  - `pandas`
  - `SQLAlchemy`
  - A MySQL database instance (for optional database integration).

### Setup:
1. Install the required Python libraries:
   ```bash
   pip install requests beautifulsoup4 pandas selenium sqlalchemy mysql-connector-python
