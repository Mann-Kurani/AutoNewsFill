## AutoNewsFill


This project automates the filling of a Google form with scraped news articles and their summaries using Selenium and Google AI's Gemini language model. It was originally developed to tackle an internship task of manually entering details for 1000 news articles!

### Features

* Scrapes news articles from a target website (currently The Times of India).
* Uses Gemini to summarize each article in 100 words.
* Categorizes each article into one of 18 news categories using Gemini.
* Fills a Google form with the article title, source, date, headline, content, summary, and category.
* Reduces manual data entry for large datasets.

### Getting Started

1. **Install dependencies:**

```bash
pip install selenium beautifulsoup4 requests google-generativeai
```

2. **Replace `"MY_API_KEY"` with your actual Gemini API key:**

- Open `newscraper TOI.ipynb` and edit the `genai.configure(api_key="MY_API_KEY")` line.
- You can obtain your API key from [https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)

3. **Configure form filling:**

- Edit the `fill_form` function in `newscraper TOI.ipynb` to match your target Google form layout (XPaths for input fields).


### Customization

* Modify the target website URL and data extraction logic in `newscraper TOI.ipynb`.
* Adjust the summarization length and category classification by editing the `generation_config` dictionary.
* Adapt the `fill_form` function to match different Google form structures.

### Disclaimer

This is a sample project for educational purposes. It may require adjustments to work with specific websites and forms. Remember to use APIs and scrape data responsibly, respecting website terms and conditions.

### Contribution

Feel free to fork this project and contribute with improvements or new features!
