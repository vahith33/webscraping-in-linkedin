## LinkedIn Job Scraping 

This project is a Python-based tool to scrape job listings from LinkedIn, providing structured data for analysis, filtering, or integration into other systems.  

## Features  

**Automated scraping**: Collect job postings based on keywords, location, and other filters.  
**Data export**: Save scraped data in CSV or JSON format for further analysis.  
**Job details**: Retrieve information such as job title, company, location, posting date, and job description.  
**Flexible configuration**: Easily modify search criteria through the script.  
**Captcha detection**: Pauses scraping when LinkedIn triggers captchas (requires manual intervention).  



## Requirements  

- Python 3.8+  
- LinkedIn account (for access)  
- **Libraries**:  
  - `selenium`  
  - `beautifulsoup4`  
  - `pandas`  
  - `requests`  

Install dependencies using:  
```bash  
pip install -r requirements.txt  
```  

---

## Setup  

1. **Clone the repository**:  
   ```bash  
   git clone https://github.com/your-username/linkedin-jobscraping.git  
   cd linkedin-jobscraping  
   ```  

2. **Configure WebDriver**:  
   - Download the appropriate [WebDriver](https://www.selenium.dev/documentation/webdriver/) for your browser.  
   - Place it in the project directory and update its path in the script.  

3. **Login to LinkedIn**:  
   - Update `config.py` with your LinkedIn credentials (*Ensure your credentials are secure!*):  
     ```python  
     USERNAME = "your_email@example.com"  
     PASSWORD = "your_password"  
     ```  

---

## Usage  

1. **Run the scraper**:  
   ```bash  
   python linkedin_scraper.py --keyword "Data Scientist" --location "New York"  
   ```  

   - Available options:  
     - `--keyword`: Specify job title or keyword (e.g., "Python Developer").  
     - `--location`: Set location (e.g., "San Francisco").  

2. **Output**:  
   - The scraped job data is saved as `output.csv` in the project directory.  

---

## Notes  

- LinkedIn's anti-scraping measures (e.g., rate limits, captchas) may block repeated or aggressive scraping. To mitigate:  
  - Use delays between requests.  
  - Rotate IPs or use a VPN.  
  - Ensure you comply with LinkedIn’s terms of service.  

---

## Contributing  

Contributions are welcome! Feel free to fork this repository, make improvements, and submit a pull request.  

---

## License  

This project is licensed under the MIT License.  

---  
