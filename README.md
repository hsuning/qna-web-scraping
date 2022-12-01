# FAQ/QnA Web Scraping

The goal of this project is to scrape question-answer pairs data on the internet


## Folder Structure
    .
    ├── data                    # Data generated by notebooks
    ├── WebScraping.ipynb       # Codes with solution explainations
    ├── WebScraping.html        # HTML version of codes with solution explainations
    ├── LICENSE
    └── README.md

## Built With
This section list all frameworks/libraries used.
- pandas==1.4.4
- requests
- bs4

<!-- GETTING STARTED -->
## Getting Started

### Scrapping
You can find the details in the notebook.
1. Setup a list of startings urls

```
starting_urls = ["https://www.zurich.co.uk/insurance/faqs"]
```

2. Initialize a storage folder with name 'website'

```
build_input_urls_storage(starting_urls, website="zurich")
```

3. Start scrapping

```
parsed_data_path = crawl_url_and_content(root='https://www.zurich.co.uk/insurance/faqs', website="zurich")

```

## License
Distributed under the MIT License. See `LICENSE.txt` for more information.
