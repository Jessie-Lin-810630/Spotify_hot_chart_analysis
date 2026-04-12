# Purpose
Web scraping the Spotify Web API and chart website to analyze the top Japan/Korean music in recent 3 months.

# Backgoud
Small project for 1-month in ccClub Python Fall 2025.

# Architecture
    - Environment: Google Colab Jupyter Notebook and link to google drive.
    - Scripts:
    ```
    project/
    ├── N01_spotifychart_xxxx.ipynb # (Extract) Download the weekly ranking chart of 
    |                                 articles in Japan/Korea and Global via 
    |                                 python-Selenium modules. The login initially 
    |                                 needed to be completed by manually and Selenium 
    |                                 will take over the following tasks.
    |
    ├── N02_csv_extract_xxxx.ipynb # Define a function cleaning the csv files obtained 
    |                                 from N01_xxx.ipynb to get unique track ID. Use 
    |                                 them to call Spotify Web Developer API for 
    |                                 features of each track.
    |
    ├── N03_API_general_xxx.ipynb   # Define a function preparing the token and headers.
    |
    ├── N04_API_extract_xxx.ipynb   # (Extract) Call the functions defined in N02 
    |                                 and N03, requesting Spotify Web Developer API for 
    |                                 track features and saved in csv files.
    |   
    └── N05_Data_Visualization.ipynb    # (Clean and Transform) Clean the data, then 
                                          analyze by using matplotlib and seaborn.
    
    ```
# Tech. Stacks
    - Python - Selenium, Requests, Pandas, Matplotlib, Seaborn
    - Data Storage - Google drive
