# Find Job

## Overview
This Python script is designed to help you search for job listings related to data science on the Indeed job search platform. It utilizes web scraping techniques to extract job information and store it in a CSV file for further analysis.

## Prerequisites
Before running the script, make sure you have the following prerequisites installed:
- Python: You should have Python installed on your system.
- Selenium: You can install it using `pip install selenium`.
- BeautifulSoup: You can install it using `pip install beautifulsoup4`.
- ChromeDriver: Download and install ChromeDriver compatible with your Chrome browser version. Ensure it's in your system's PATH.

## How To
1. Clone or download this script to your local machine.

2. Ensure you have all the prerequisites mentioned above installed.

3. Modify the script if needed:
   - You can customize the job search query by changing the URL in the `self.driver.get(...)` line inside the `__init__` method. The example query searches for "data science" jobs in the United States. You can adjust the query parameters as per your requirements.

4. Run the script by executing it using Python: `python job_search.py`

5. The script will open a Chrome browser window, perform the job search, and scrape job listings from the Indeed website.

6. It will collect job information such as job title, location, company name, and salary (if available). This data will be displayed in the terminal as the script runs.

7. The script will also attempt to click on each job listing to reveal more details, but this part of the code is currently commented out. You can uncomment and modify it as needed to scrape additional information.

8. The scraped job data will be stored in a CSV file named "jobs.csv" in the same directory as the script.

## Important Notes
- Please be aware that web scraping might be subject to terms of service of the website you are scraping from. Ensure that you are allowed to scrape data from Indeed before using this script for any significant scraping operation.

- The script may need adjustments if the structure of the Indeed website changes, as it relies on specific HTML elements for data extraction.

- Depending on your internet connection and the number of job listings you want to scrape, the script may take some time to run. Adjust the `sleep` durations in the code if necessary.
