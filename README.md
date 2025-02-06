# AI-Web-Scraper-DeepSeek-Crawl4AI

DeepSeek Crawler is a Python-based web scraper that extracts venue data (e.g., wedding reception venues) using **Crawl4AI** and **LLM-based extraction**. The collected data is saved in CSV format.

## Features

- **Asynchronous web crawling** with [Crawl4AI](https://pypi.org/project/Crawl4AI/)
- **LLM-powered data extraction** for accurate parsing
- **CSV export** for structured data storage
- **Modular and simple architecture**, making it easy to modify

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/sabahatatta/AI-Web-Scraper-DeepSeek-Crawl4AI.git
   cd AI-Web-Scraper-DeepSeek-Crawl4AI

	2.	Install dependencies:

pip install -r requirements.txt



Usage

Run the crawler with:

python main.py

Project Structure

.
├── main.py            # Main entry point
├── config.py          # Configuration settings (Base URL, CSS selectors, etc.)
├── models/
│   └── venue.py       # Defines the Venue data model
├── utils/
│   ├── data_utils.py  # Functions for processing & saving data
│   └── scraper_utils.py  # Functions for crawling setup & execution
├── requirements.txt   # Required dependencies
└── README.md          # Documentation

Configuration

Modify config.py to update:
	•	Base URL for scraping
	•	CSS selectors for extracting relevant data
	•	Output file settings

Output

Extracted data is saved as venues.csv.

License

This project is open-source and available under the MIT License.

This version keeps it **clear, concise, and easy to follow**, while maintaining all essential details. Let me know if you need any modifications! 🚀 |oai:code-citation|