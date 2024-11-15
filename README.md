
# AI Web Scraper

An AI-powered web scraping tool that utilizes **Ollama**, **BrightData**, **Selenium**, and other libraries to scrape, analyze, and summarize web pages. This scraper is designed to gather structured data from websites and use AI models to process and analyze that data for various use cases.

## Features

- **AI-Powered Scraping**: Use AI models like **Ollama** to process and analyze scraped data.
- **Web Scraping**: Gather data from websites using libraries like **Selenium** for dynamic content.
- **Smart Proxy Management**: Use **BrightData** for managing proxies to handle scraping at scale.
- **Content Summarization**: Summarize and analyze content using AI-based language models.

## Libraries & Tools

- **Ollama**: AI model for content analysis and summarization.
- **BrightData (formerly Luminati)**: Proxy management for scalable scraping.
- **Selenium**: Automated browser interaction for dynamic content scraping.
- **BeautifulSoup**: HTML parsing to extract relevant information.
- **Requests**: Simple HTTP requests for static content scraping.

## Installation

To set up this project locally, follow the steps below.

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/ai-web-scraper.git
cd ai-web-scraper
```

### 2. Create a Virtual Environment

(Optional but recommended)

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Setup API Keys

You will need to set up API keys for **Ollama** and **BrightData** to use their services. Create an `.env` file in the root of the project and add the following:

```env
OLLAMA_API_KEY=your_ollama_api_key
BRIGHTDATA_API_KEY=your_brightdata_api_key
```

### 5. Run the Application

```bash
python app.py
```

## Usage

Once the application is set up, you can start using it to scrape web pages. The basic flow is:

1. Input a URL to scrape.
2. The scraper will gather content from the page.
3. The data is processed by an AI model (Ollama) to summarize or extract relevant information.
4. The final result is displayed or stored.

### Example

```bash
Enter the URL to scrape: https://example.com
Scraping the website: https://example.com
Summarized content:
"Example website content summary"
```

## Code Structure

- **app.py**: Main file for scraping and AI analysis.
- **scraper.py**: Handles the web scraping logic using Selenium and BeautifulSoup.
- **ai_analysis.py**: Contains logic to process scraped content using AI models.
- **proxy_manager.py**: Manages proxy rotation with BrightData.
- **requirements.txt**: Lists all Python dependencies.
- **.env**: Stores API keys and other environment variables.

## Dependencies

- `Ollama`: For content analysis and summarization.
- `Selenium`: For dynamic content scraping.
- `BeautifulSoup`: For HTML parsing.
- `Requests`: For static web scraping.
- `BrightData`: For proxy management.
- `dotenv`: To manage environment variables.
- `pandas`: (Optional) For organizing and storing scraped data.

Install the required dependencies using:

```bash
pip install -r requirements.txt
```

## Troubleshooting

- **Selenium Errors**: Make sure you have installed the correct WebDriver for your browser (e.g., ChromeDriver for Chrome).
- **API Errors**: Ensure that you have valid API keys in the `.env` file.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to adjust the instructions, such as adding specific examples, usage cases, or additional setup details.
