# Highest-Grossing Japanese Films Scraper

A simple Python web scraping project that extracts data from Wikipedia's list of highest-grossing Japanese films and saves each table into a separate CSV file.

## Overview

This project uses Python, `requests`, `BeautifulSoup`, and `pandas` to:

- fetch the target Wikipedia page,
- parse the HTML tables,
- clean the extracted values,
- export the resulting data into CSV files.

## Features

- Automated data extraction from a public Wikipedia page
- Support for multiple tables on the same page
- CSV export for each discovered table
- Lightweight, beginner-friendly Python implementation

## Project Structure

- `Scraping.py` — main scraper script
- `README.md` — project documentation
- Generated CSV files — output data files saved in the repository directory

## Requirements

Make sure you have Python 3 installed, then install the required dependencies:

```bash
pip install requests beautifulsoup4 pandas lxml
```

## Installation

1. Clone the repository:

```bash
git clone https://github.com/Not-Just-Pratul/Web-Scraping-for-Beginners.git
cd Web-Scraping-for-Beginners
```

2. Install the dependencies:

```bash
pip install requests beautifulsoup4 pandas lxml
```

3. Run the script:

```bash
python Scraping.py
```

## Usage

When you run the script:

- it sends a request to the Wikipedia page,
- parses the available HTML tables,
- extracts the header and row content,
- saves the data into files named:

```text
highest-grossing-japanese-films-table-1.csv
highest-grossing-japanese-films-table-2.csv
```

The output files are created in the same directory where the script is executed.

## Notes

- Ensure you have write permissions for the folder where the CSV files are created.
- If the script fails, check the terminal output for any errors or HTTP issues.
- Wikipedia pages may change over time, so the scraper may need occasional updates if the site structure changes.

## How It Works

The scraper follows this workflow:

1. Define the target URL.
2. Send an HTTP GET request.
3. Parse the HTML with BeautifulSoup.
4. Locate the relevant wiki tables.
5. Extract headers and row values.
6. Convert the data into a pandas DataFrame.
7. Export the data to CSV files.

## Contributing

Contributions are welcome. If you would like to improve the scraper or documentation, please open a pull request with a concise description of the changes.

## Acknowledgments

- Wikipedia for providing the source data
- `requests`, `BeautifulSoup`, `pandas`, and `lxml` for supporting the scraping workflow