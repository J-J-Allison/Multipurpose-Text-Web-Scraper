# Multipurpose-Text-Web-Scraper
Python script that crawls a website, extracts all text from every subpage (including navigation), and saves it to a file. Includes interactive prompts for URL, domain limits, request delays, and page limits.

## Features

- Interactive URL input with validation
- Crawls entire domain (respects domain boundaries)
- Extracts all text from each page
- Configurable request delays (polite to servers)
- Page limit to prevent runaway crawls
- Saves results to text file
- Error handling for failed requests

## Installation
```bash
pip install requests beautifulsoup4
```

## Usage
```bash
python scraper.py
```

Follow the prompts to enter:
- Website URL (e.g., `https://example.com`)
- Domain to crawl (optional custom domain)
- Delay between requests (default: 1 second)
- Output file option (default: `scraped_content.txt`)
- Max pages to scrape (0 = unlimited)

## Example
```bash
$ python scraper.py
Enter the website URL: https://example.com
Domain detected: example.com
Scrape only this domain? (y/n): y
Enter delay in seconds: 1
Save output to file? (y/n): y
Max pages: 0
```

## Notes

- Respect `robots.txt` and site terms of service
- Delays prevent server overload
- For JavaScript-heavy sites, use Selenium instead
- Check site policies before scraping
