# AI-Web-Scraper-DeepSeek-Crawl4AI

**DeepSeek Crawler** is a powerful, Python-based web scraper designed to extract venue data (e.g., wedding reception venues) using **Crawl4AI** for asynchronous crawling and **LLM-based extraction** for intelligent parsing. The collected data is efficiently stored in a structured CSV format, making it easy to analyze and utilize.

## 🌟 Features

- **Asynchronous Web Crawling**: Utilizes [Crawl4AI](https://pypi.org/project/Crawl4AI/) for high-performance, non-blocking web scraping.
- **LLM-Powered Data Extraction**: Leverages advanced language models for accurate and context-aware data parsing.
- **CSV Export**: Saves extracted data in a clean, structured CSV format for seamless integration with analytics tools.
- **Modular Architecture**: Designed with simplicity and extensibility in mind, allowing users to easily customize and enhance functionality.
- **Environment-Friendly Configuration**: Securely store sensitive keys in `.env` files, ensuring safe and organized project management.

---
## 🛠️ Tech Stack

### Core Libraries

- **Crawl4AI**: A robust library for asynchronous web crawling and data extraction.
- **Python**: The backbone of the project, providing flexibility and ease of use for both beginners and advanced developers.
### Data Handling
- **Pandas**: Handles structured data manipulation and ensures efficient CSV export.
### LLM Integration
- **LLM Models**: Employs state-of-the-art language models to extract and process data with precision and context awareness.

---
## 📂 Project Structure


├── main.py            # Main entry point for running the scraper
├── config.py          # Configuration settings (Base URL, CSS selectors, etc.)
├── models/
    └── __init__.py
│   └── venue.py       # Defines the Venue data model for structured representation
├── utils/
    └── __init__.py
│   ├── data_utils.py  # Utility functions for processing and saving data
│   └── scraper_utils.py  # Functions for setting up and executing the crawler
├── requirements.txt   # Lists all required Python dependencies
├── .env               # Environment variable file for securely storing API keys
├── venues.csv         # Output file containing the extracted venue data
└── README.md          # Comprehensive documentation for the project


---
## ⚙️ Application Workflow 

### 1. Configuration

- Update `config.py` to define:
  - **Base URL**: The website URL from which data will be scraped.
  - **CSS Selectors**: Target specific HTML elements for data extraction.
  - **Output Settings**: Customize the output file name and format (e.g., `venues.csv`).

### 2. Crawling and Extraction

- The scraper uses **Crawl4AI** to asynchronously fetch web pages, ensuring fast and efficient data retrieval.
- Extracted raw data is processed using **LLM-based extraction**, ensuring accuracy and contextual relevance.
- Structured data is then saved in CSV format using **Pandas**, making it ready for analysis or further processing.

### 3. Execution

- Run the scraper with the following command:
  ```bash
  python main.py
  ```
- The extracted data will be saved as `venues.csv` in the project directory, ready for immediate use.

---
## 🔧 Setup Instructions

### Prerequisites

- **Python 3.9 or later**: Ensure you have Python installed on your system.
- **Internet Connection**: Required for web scraping and accessing external APIs.

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
3. **Set Up Environment Variables**:
   Create a `.env` file in the root directory and add your API keys:
   ```env
   GROQ_API_KEY=your_groq_api_key_here
   ```
4. **Run the Scraper**:
   ```bash
   python main.py
   ```
   - The scraper will start crawling the specified website and save the extracted data as `xyz.csv`.

---
## 🚀 Future Enhancements

- **Support for Additional Data Formats**: Extend support for JSON, Excel, and other formats to cater to diverse use cases.
- **Advanced Error Handling**: Implement retry mechanisms and robust error handling to ensure smooth operation even in challenging scenarios.
- **Parallel Processing**: Optimize crawling speed by leveraging parallel processing techniques.
- **Dynamic Website Support**: Integrate headless browsers to scrape data from JavaScript-heavy websites.

---
## 🤝 Contributing

Contributions are highly encouraged! To contribute:

1. Fork the repository.
2. Create a new branch (`feature/your-feature-name`).
3. Commit your changes and push to the branch.
4. Open a pull request with a detailed description of your enhancements.

---
## 📜 License

This project is open-source and available under the **MIT License**.

---
Feel free to reach out for feedback or suggestions to make this project even better! 😊
```