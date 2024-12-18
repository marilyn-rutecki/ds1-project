# PPOL 5203 - Clicks and Crimes: Analysis of Crime Coverage in Washington, D.C.


This repository contains the final project for Data Science I: Foundations.

## Project Contents 

### Overview/ Abstract

This study investigates the digital landscape of crime communication in Washington, D.C. and analyzes how crime stories are reported and discussed across social media and mainstream news platforms. We scraped and downloaded data from YouTube, Fox News 5, and the Metropolitan Police Department (MPD). Using aggregate statistics, predictive and inferential modeling, and sentiment analysis, we analyzed coverage of crime-related content, comparing it with MPD crime statistics. Our research explored three hypotheses: the likelihood of media coverage based on the crime type (with violent crimes expected to receive more attention), geographical variations in crime reporting across D.C. quadrants, and the potential influence of personal characteristics on content engagement and coverage. We discovered egregious crimes like homicide and assault garner more media attention, with nuanced geographical reporting patterns emerging—particularly in wealthier neighborhoods like Northwest D.C. Contrary to initial expectations, crimes committed by teenagers did not consistently drive media engagement. This analysis contributes to understanding crime narratives in D.C. and could be further applied to broader media coverage and engagement. 

### Installation & Getting Started

Install the following necessary Python Packages: 
- googleapiclient: For interacting with Google APIs.
- pandas: For data manipulation and analysis.
- matplotlib: For plotting visualizations.
- numpy: For numerical computations.
- scikit-learn: For machine learning algorithms and data preprocessing.
- python-dotenv: For loading environment variables from .env files.
- praw: For accessing Reddit’s API.
- requests: For sending HTTP requests.
- beautifulsoup4: For web scraping HTML content.
- statsmodels: For statistical models and tests.
- transformers: For sentiment analysis of text data.
- tensorflow: To operationalize transformers for sentiment analysis.
- XGBoost: For multilabel machine learning classification 

Beyond installing the libraries listed above, make sure that you have the necessary API keys set up for the respective libraries like the Youtube API and Reddit API before running the project.


### Documentation

Each of the jupyter notebook files contain codes with a procedural guide on running them. The codes are commented and grouped into chunks to make it easier to understand the process of data collection and visualization. 

### Contributing

For anyone interested in contributing to our project, please feel free to send a pull request and we will approve it. Feel free to also reach to use by email or direct message if you identify or notice any bugs that we could fix to make the project better. 

### Acknowledgements

This project is a collective work of three Data Science I students: Josahn Oginga, Muhammada Saad, and Marilyn Rutecki under the professorship of Prof. Tiago Ventura. The project utilized chatGPT to identify in developing robust dictionaries such as crime category and Washington DC names that were very instrumental in our data collection process. 

### License

This project is open for public use, and anyone is encouraged to utilize, modify, and distribute it to advance the public good. We ask that you acknowledge the original authorship and respect the ethical use of the project. While the project is provided as-is without warranty, we encourage its use for positive societal impact, including in areas of social research, education, and community development. Please ensure your use aligns with ethical standards and contributes to meaningful outcomes. 

### Folders and Files:

This project contains the following folders and files. 

#### **Jupyter Notebooks**
- **`FOX_5_DC_Scraper_Analysis.ipynb`**: Scrapes FOX 5 DC stories and provides analysis, including relevant graphical representation, sentiment analysis, etc.  
- **`Youtube API.ipynb`**: Extracts data using the YouTube API.  
- **`Youtube Analysis.ipynb`**: Analyzes and visualizes YouTube crime data.  
- **`mpd-data.ipynb`**: Includes MPD (Metropolitan Police Department) data analysis of the MPD crime database  
- **`reddit-scrape.ipynb`**: Scrapes Reddit posts using PRAW wrapper.  

#### **Data Files**
- **`FOX5_DC_News_Raw.csv`**: Dataset containing all FOX 5 DC news stories from September 1 2024 till December 5 2024.
- **`FOX5_crime_related_news.csv`**: Dataset containing crime related news stories from FOX 5 based on the defined list of crime related keywords.
- **`FOX5_labeled_sampled_stories.csv`**: Dataset containing 50 news stories randomly sampled from the original FOX 5 crime related news stories dataset for manually coding for type of crime, locality, and personal attributes.
- **`dc-crimes-search-results.csv`**: Raw MPD data.  
- **`filtered_reddit_posts.csv`**: Pre-processed Reddit posts dataset.  
- **`last_year_posts.csv`**: Reddit posts from the past year.  
- **`reddit_test_submission_db.csv`**: Test submissions dataset for Reddit.  
- **`updated_file.csv`**: Updated dataset file and processed data from MPD.  
- **`year_posts.csv`**: Yearly Reddit post data.  
- **`yt-crime_data_2.csv` / `yt_crime_data_2.csv`**: YouTube video datasets meeting search parameters.  

#### **Output**
- **`crime_types_percentage.jpg`**: Visualization of crime type percentages.  
- **`locality_percentage.jpg`**: Visualization of locality crime percentages.
- **`crime_type_comparison.jpg`**: Comparative graph on types of crime for MPD, YouTube and FOX 5.
- **`locality_comparison.jpg`**: Compares incidence/reporting of crime for MPD, YouTube and FOX 5.
- **`personal_attributes_comparison.jpg`**: Compares personal characteristics for perpetrators/victims in crime related coverage for YouTube and FOX 5.
- **`FOX5_sentiment_distribution.jpg`**: Sentiment analysis for FOX 5 crime related news stories. 

#### **Configuration and Miscellaneous**
- **`.gitignore`**: Specifies files to ignore in version control. This file contains API keys stored in a local .env file  
- **`.DS_Store`**: System file (for macOS).  

#### **Other**
- **`README.md`**: Project overview and documentation.   


Thank you!!








