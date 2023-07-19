# scraping_mars_challenge
by Panfilo Marbibi  

# Contents:
- mars (dir)
  - part_1_mars_news.ipynb
  - part_2_mars_weather.ipynb
  - output  (dir)
    - mars_articles.json
    - mars_data.csv
   
# Summary
- This project scrapes data from websites using splinter and BeautifulSoup.
- part_1_mars_news.ipynb
    - This Jupyter Notebook scrapes data from 'https://static.bc-edx.com/data/web/mars_news/index.html'
    - First, it scrapes the main body of the website that contains text
    - Next, it uses the scraped data to pull the article names and article summaries.
    - Article names and summaries are then stored in a list of dictionaries, labeling the title and summary.
    - The list is then saved into a JSON file in the "output" folder for later use
- part_2_mars_weather.ipynb
    - This Jupyter Notebook scrapes the table from "https://static.bc-edx.com/data/web/mars_facts/temperature.html"
    - Using BeautifulSoup, this takes the table and stores it into a variable
    - The notebook will then gather the column names of the table
    - Next, the notebook will gather the rows that correspond to the column names
    - The column names and rows are then placed in a Pandas DataFrame
    - The notebook will make sure to assign the proper variable types for the columns of the data frame
    - The notebook is then tasked to use the data in the data frame to answer the following questions
      - "How many months are there on Mars?"
      - "How many Martian days' worth of data are there?"
      - "What is the average low temperature by month?"
      - "Average pressure by Martian month"
      - "How many terrestrial (earth) days are there in a Martian year?"
    - The notebook also constructs a bar graph to visualize the average low temperatures, by month, on Mars
    - The notebook also constructs a bar graph to visualize the average atmospheric pressure, by month, on Mars
    - The above graphs are also reconstructed and ordered in ascending order to show which month has the lowest average temperature, and which month has the highest average temperature.
    - A graph in ascending order is also constructed to show which months have the lowest atmospheric pressure and which months have the highest atmospheric pressure on average
    - A graph of the number of terrestrial days recorded vs the minimum temperatures is constructed to calculate the number of terrestrial days (on Earth) equal to a year on Mars, or a full revolution around the Sun of Mars, by taking the distance from peak to peak.
    - The notebook then saves the data into a CSV file in the "output" folder for later use
 
--Coding used was derived from classroom activities
