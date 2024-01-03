# Amazon Web Scraping Project

## Overview

This project involves web scraping data from Amazon to track the price of a specific product over time. The product in question is a T-shirt related to data analysis. The script connects to the Amazon website, extracts relevant information such as product title and price, and stores it in a CSV file. Additionally, the project includes functionality to send an email notification if the price falls below a certain threshold.

## Key Steps

### 1. Importing Libraries

The necessary libraries, including BeautifulSoup, requests, time, and datetime, are imported to facilitate web scraping and other functionalities.

### 2. Connecting to the Website

The script connects to the Amazon website using the provided URL and sets up headers for the request.

### 3. Extracting Data

BeautifulSoup is used to parse the HTML content, extract relevant information such as product title and price, and store it in variables.

### 4. Cleaning and Storing Data

The extracted data, including the title, price, and current date, is cleaned and stored in a CSV file named 'AmazonWebScraping.csv.'

### 5. Checking Price and Sending Email Notification

The script includes a function, `check_price()`, that runs in a loop, periodically checking the product price. If the price falls below $15, an email notification is sent using the `send_mail()` function.

### 6. Continuous Monitoring

The script runs continuously, checking the price and updating the CSV file every 24 hours (86400 seconds).

This project demonstrates the use of web scraping, data extraction, CSV handling, and email notification functionality for tracking product prices on e-commerce platforms.
