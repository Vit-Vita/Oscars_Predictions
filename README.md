# 📽 Oscars Winners Predictions

In this project, we worked as a team of three students to extract, integrate, pre-process and transform data to produce a report answering a research question.  

As Student B, I was tasked with scraping critics' reviews for films that won the Academy Awards or were nominated from 2009 until 2024 as well as their characteristics (director, producer, runtime, cast and crew, etc.) from the website Rotten Tomatoes (URL of the main page : https://www.rottentomatoes.com/)

We ultimately analysed this data to try to better understand what criteria are used to choose an Oscar winner from amongst the nominees.


Programming Languages and Libraries : Python 3, Pandas, Matplotlib, RegEx, pickle, NLTK, Scikit-Learn, matplotlib.pyplot

Web scraping tools: BeautifulSoup, Selenium, ChromeDriver, Requests

Database and storage : MariaDB, SQLAlchemy, SWITCH Drive

Additional tools: Jupyter Notebook, API Requests, Linux Virtual Machine


## The contents of the repository are organized as follows:

### 1. "Code" folder:

   a. CIP_Rottentomatoes_COMMENTED_FULL_VERSION which contains the full Python code (parts 1, 2 and 3 below) with detailed comments
   
   b. CIP_Rottentomatoes_part_1_scraping_and_cleaning which contains only the code for scraping and cleaning the data 
   
   c. CIP_Rottentomatoes_part_2_enrichment which enriches the data with further calculations and information
   
   d. CIP_Rottentomatoes_part_3_upload which contains code for uploading the cleaned and enriched data to a database (MariaDB)
   
   e. "Data" folder to be able to run the code

   f. CIP_Group_Work_Analysis which shows the code used for answering some of the questions of the final group report

### 2. "Data" folder:

    a. Stage 1 data resulting from the extraction. This is the metadata of the movies and their reviews as they were extracted
    
    b. Stage 3 data which contains the final version of the data ready to be used for analysis after cleaning and enrichment

The resulting data is not contained in the repository because of the size of the files. The cleaned and enriched data from Students A and C were merged using the movie titles as the merging key. For Student B’s data, aggregation and pivoting was performed to consolidate each row representing one critic review, into one row per movie encapsulating all critic reviews. It was then also merged using the movie title.
