Project Report: Amazon Web Scraper with Price Tracking and Email Notification

1. Introduction:

The aim of this project is to develop a Python script for scraping product data from Amazon, specifically targeting the title and price of a chosen product.
The script is designed to periodically check for changes in price and store the data in a CSV file.
Additionally, the project includes functionality to notify the user via email when the price of the product drops below a certain threshold.

2. Project Overview:

The project utilizes Python along with several libraries, primarily BeautifulSoup and requests for web scraping, pandas for data manipulation, and smtplib for email functionality.
3. Script Components:

a. Web Scraping:

The script sends an HTTP request to the Amazon product page and extracts relevant information using BeautifulSoup.
It targets specific HTML elements, such as the product title and price, using their IDs.
The data is cleaned and formatted before being stored.


b. CSV File Handling:

The script writes the scraped data into a CSV file named "AmazonWebScraperDataset.csv".
It utilizes the csv module to handle file operations efficiently.
Data is appended to the CSV file with each execution, allowing for historical price tracking.


c. Email Notification:

The script defines a function for sending email notifications when the price drops below a predefined threshold.
However, the email sending functionality is incomplete and requires further implementation.
SMTP (Simple Mail Transfer Protocol) is used for sending emails, with the script connecting to Gmail's SMTP server.


d. Automation:

The script utilizes a while loop to continuously execute the price-checking function at regular intervals.
It uses time.sleep() to introduce delays between successive executions, ensuring efficient resource utilization.


4. Future Improvements:

Implement complete email sending functionality within the send_mail() function.
Enhance error handling to gracefully handle exceptions during web scraping and email sending.
Add support for tracking multiple products simultaneously.
Incorporate logging to record script activity and facilitate debugging.
Introduce user-defined thresholds for price monitoring and notification.


5. Conclusion:

The project successfully demonstrates the capabilities of web scraping for data extraction from online platforms like Amazon.
With further development, it can serve as a valuable tool for price tracking and alerting users to favorable purchasing opportunities.
Continuous refinement and enhancement will ensure its effectiveness and reliability in real-world scenarios.


6. References:

BeautifulSoup
requests 
pandas 
smtplib 
This report provides an overview of the Amazon web scraper project, highlighting its functionality, components, and potential areas 
for improvement. Further development and refinement will enhance its utility and effectiveness in real-world applications.
