# AI-Web-Scraper-DeepSeek-Crawl4AI

DeepSeek Crawler is a Python-based web scraper that extracts venue data (e.g., wedding reception venues) using **Crawl4AI** and **LLM-based extraction**. The collected data is saved in CSV format.

---
## 🌟 Features

- **Asynchronous web crawling** with [Crawl4AI](https://pypi.org/project/Crawl4AI/)
- **LLM-powered data extraction** for accurate parsing
- **CSV export** for structured data storage
- **Modular and simple architecture**, making it easy to modify
---

## 🛠️ Tech Stack

### Core Libraries
- **Crawl4AI**: For asynchronous web crawling and data extraction.
- **Python**: Powers the entire scraping and data processing pipeline.
### Data Handling
- **Pandas**: Used for structured data manipulation and CSV export.
### LLM Integration
- **LLM Models**: Enable intelligent and accurate data extraction from web pages.
---

## 📂 Project Structure
```

├── main.py            # Main entry point for running the scraper
├── config.py          # Configuration settings (Base URL, CSS selectors, etc.)
├── models/
│   └── venue.py       # Defines the Venue data model
├── utils/
│   ├── data_utils.py  # Functions for processing & saving data
│   └── scraper_utils.py  # Functions for crawling setup & execution
├── requirements.txt   # Required dependencies
├── .env               # environment variable file(Store keys) 
├── venues.csv 
└── README.md          # Documentation
```
---

## ⚙️ Application Workflow

### 1. Configuration
- Update `config.py` to define:
  - Base URL for scraping.
  - CSS selectors for extracting relevant data.
  - Output file settings (e.g., `venues.csv`).

### 2. Crawling and Extraction
- The scraper uses **Crawl4AI** to asynchronously fetch web pages.
- Extracted raw data is processed using **LLM-based extraction** for accuracy.
- Structured data is then saved in CSV format using **Pandas**.

### 3. Execution
- Run the scraper with the command:
  ```bash
  python main.py
  ```
- The extracted data will be saved as `venues.csv` in the project directory.
---

## 🔧 Setup Instructions

### Prerequisites
- Python 3.9 or later
- Internet connection for web scraping

### Steps
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/sabahatatta/AI-Web-Scraper-DeepSeek-Crawl4AI.git
   cd AI-Web-Scraper-DeepSeek-Crawl4AI
   ```
2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Scraper**:
   ```bash
   python main.py
   ```
   - The scraper will start crawling and save the extracted data as `venues.csv`.
---

## Future Enhancements
- Add support for additional data formats (e.g., JSON, Excel).
- Integrate advanced error handling and retry mechanisms.
- Optimize crawling speed with parallel processing.
- Add support for dynamic websites using headless browsers.
---

## 🤝 Contributing

Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch (`feature/your-feature-name`).
3. Commit your changes and push to the branch.
4. Open a pull request.
---

## 📜 License

This project is open-source and available under the MIT License.
---
Feel free to reach out for feedback or suggestions to make this project even better! 😊
```