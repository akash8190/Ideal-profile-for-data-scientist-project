# Ideal Profiles

![alt text](https://d.novoresume.com/images/blogs/ac8c93c0-5759-11e8-9417-7d5200ef4edd/bg-cover-article.png)


What does an ideal Data Scientist's profile look like? This project aims to provide a quantitative answer based on job postings. In this project, I scraped job posting data from Indeed and analyzed frequencies for various Data Science skills. The analysis then can be used not only as objective keyword reference for resume optimization, but can also serve as Data Science learning road map!!



## How to Use
If you want to run the code locally, please download the repo and build your Anaconda environment using the `env_ideal_profiles.yaml` file, and download geckodriver (see Requirements below). Then you can start with data scraping by running `python scrape_date.py` in Anaconda Prompt. Once you have the raw data, you can then clean the data using the `data_wrangling.ipynb` Jupyter Notebook. Finally, the `ideal_profiles_2.ipynb` Notebook can be used to make various plots. Refer to list below for the roles of different files.


## Requirements
- Windows 10 OS
- Firefox Web Browser 63.0.3
- Ananconda 3
- geckodriver v0.22.0 (geckodriver-v0.22.0-win64.zip, available [here](https://github.com/mozilla/geckodriver/releases))
- pandas (see the yaml file for version number, same below)
- numpy
- matplotlib
- json
- re
- csv
- wordcloud
- nltk
- bs4 (BeautifulSoup)
- selenium


## Files
- `scrape_data.py`: scrapes the data from Indeed.ca
- `process_text.py`: performs various text related operations such as remove digits, tokenize, and check term frequency
- `helper.py`: contains data loading and various plotting functions
- `data_wrangling.ipynb`: gathers the raw text data, counts term frequency and stores the result in a pandas dataframe
- `ideal_profiles.ipynb`: creates spider plots to visualize various Data Science roles' skill requirements based on intuition
- `ideal_profiles_2.ipynb`: creates skill distribution and word cloud plots to represent ideal profiles quantitatively
- `stopwords.csv`: contains the stop words for word cloud plotting
- `env_ideal_profiles.yaml`: the Anaconda environment file for setting up the project environment



## To-do's
- Allow to query Indeed USA instead of the Canadian site and increase the number of postings to scrape
- Allow to show context for specific words in word clouds
- Update all docstrings and comments
- OOP
- Code refactoring - single responsibility principle for functions
- Add Data Analyst and AI Engineer roles
- Allow to show Percentage of Mentions for a certain skill, i.e., out of 1000 job postings, what proportion mentions the given skill?


## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Refrence
Towards data science blog end to end project



