# LinkedIn Job Crawler

This project is a LinkedIn job crawler built using Python and Selenium. It allows you to scrape job postings from LinkedIn based on specific search criteria and save the results to an Excel file.

## Prerequisites

Before running the script, make sure you have the following dependencies installed:

- Python 3.x
- Selenium
- BeautifulSoup
- pandas
- tqdm
- yaml

You can install the required dependencies using pip:
pip install selenium beautifulsoup4 pandas tqdm pyyaml

## Setup

1. Clone the GitHub repository: git clone https://github.com/KamranNiroomand/linkedin-job-crawler.git
2. Navigate to the project directory:
cd linkedin-job-crawler

3. Install the required dependencies as mentioned in the "Prerequisites" section.

4. Create a YAML configuration file named `config.yaml` in the project directory and add your LinkedIn login credentials:

```yaml
username: your_username
password: your_password
Usage

To run the LinkedIn job crawler, execute the following command:
python crawler.py
""
The script will open a Chrome browser window and automate the login process using the provided credentials. It will then navigate to the specified job search URL on LinkedIn.

By default, the script is set to scrape job postings for the "machine learning engineer" keyword. You can modify the URL in the code to search for other job titles or customize the search criteria.

The crawler will collect the job links from multiple pages of search results and store them in a list. After collecting the links, it will visit each job page and extract relevant information such as job title, company name, location, work method, post date, work time, and job description.

The scraped data will be saved to an Excel file named jobs.xlsx located in the ../data/ directory relative to the project directory. If the file already exists, it will be overwritten.





