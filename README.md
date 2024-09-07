# ScraperAI

**ScraperAI** is a web scraping and AI-based content extraction tool that enables users to scrape websites, clean HTML content, and parse specific information using an AI model (LLaMA). The system allows users to input a website URL and define what information they want to extract, and the tool will return only the requested data.

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Code Overview](#code-overview)
  - [main.py](#mainpy)
  - [scraper.py](#scraperpy)
  - [parse.py](#parsepy)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Web Scraping**: Scrape website content using Selenium and Chrome WebDriver.
- **HTML Content Cleaning**: Remove scripts, styles, and unnecessary elements using BeautifulSoup.
- **AI-Powered Parsing**: Use the LLaMA model to extract specific information based on user input.
- **Simple UI**: Built with Streamlit, providing an easy-to-use interface for non-technical users.

## Requirements

To run this project, you need the following dependencies:

- Python 3.8+
- [Streamlit](https://streamlit.io/) for the user interface
- [Selenium](https://www.selenium.dev/) for web scraping
- [BeautifulSoup4](https://www.crummy.com/software/BeautifulSoup/) for HTML parsing
- [Langchain](https://www.langchain.com/) and LLaMA model for AI-powered content parsing
- Chrome WebDriver for Selenium

You can install the necessary packages using the following command:

```bash
pip install -r requirements.txt
```

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/ScraperAI.git
   ```

2. Navigate to the project directory:

   ```bash
   cd ScraperAI
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Make sure you have Chrome WebDriver installed and configured correctly. If you haven't done that yet, you can download it [here](https://sites.google.com/a/chromium.org/chromedriver/downloads) and follow the installation guide.

## Usage

1. Start the Streamlit application:

   ```bash
   streamlit run main.py
   ```

2. Enter the website URL that you want to scrape.
3. After scraping the content, enter a description of the data you want to extract (e.g., product prices, article titles, etc.).
4. ScraperAI will use the AI model to parse the content and extract only the relevant information.

## Project Structure

The project structure follows a simple, modular format:

```bash
ScraperAI/
│
├── main.py         # Streamlit interface for user input and scraping
├── scraper.py      # Handles web scraping and content cleaning
├── parse.py        # Processes the cleaned content using the LLaMA AI model
├── requirements.txt  # Lists required Python packages
└── README.md       # Project documentation
```

## Code Overview

### `main.py`

This file is responsible for the Streamlit UI and controlling the workflow. It accepts user input, performs the scraping, and calls the parsing function to extract the required information.

### `scraper.py`

This file handles the web scraping logic using Selenium. It uses BeautifulSoup to clean up the HTML content by removing JavaScript, CSS, and other unnecessary elements.

### `parse.py`

This file leverages the LLaMA AI model to parse the cleaned HTML content. The model only returns the specific data requested by the user based on their input.

## Contributing

If you'd like to contribute to this project, feel free to submit a pull request or open an issue.

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Usage Notes:
- You should replace `"https://github.com/yourusername/ScraperAI.git"` with the actual GitHub URL of your repository.
- Add or modify instructions based on your actual project setup if any details change.
