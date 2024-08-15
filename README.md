# Mars-Data-Web-Scraping
Summary for the Web Scraping and Data Analysis Project:
Part 1: Scrape Titles and Preview Text from Mars News
In this part of the project, we utilized automated browsing and Beautiful Soup to scrape the Mars News website. We identified and extracted the titles and preview text of the news articles, storing the data in Python dictionaries with keys for title and preview. The scraped data was then organized into a list and printed in the Jupyter Notebook. Additionally, an option to export the data to a JSON file was provided for easier sharing.
Part 2: Scrape and Analyze Mars Weather Data
For the second part of the project, we used automated browsing and Beautiful Soup to scrape Mars weather data from a specific URL. The data was assembled into a Pandas DataFrame with columns representing various parameters such as id, terrestrial date, sol, ls, month, min_temp, and pressure. We analyzed the dataset using Pandas functions to answer key questions such as the number of months on Mars, the number of Martian days worth of data, the coldest and warmest months on Mars, the months with the lowest and highest atmospheric pressure, and the approximate number of terrestrial days in a Martian year. Visualizations, including bar charts, were used to present the analysis results effectively.
This project enhanced our web scraping skills, data extraction techniques, and data analysis capabilities, providing valuable insights into Mars news and weather data.



To complete this project, you'll follow a structured approach to web scraping and data analysis using Python. Here's a step-by-step guide on how to approach each part of the challenge:
Part 1: Scrape Titles and Preview Text from Mars News
Open the Jupyter Notebook in the starter code folder named part_1_mars_news.ipynb. You will work in this code as you follow the steps below to scrape the Mars News website.

Use automated browsing to visit the Mars news siteLinks to an external site.. Inspect the page to identify which elements to scrape.
Create a Beautiful Soup object and use it to extract text elements from the website.

Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:

Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. 
Store all the dictionaries in a Python list.

Print the list in your notebook.

Optionally, store the scraped data in a file (to ease sharing the data with others). To do so, export the scraped data to a JSON file. (Note: there will be no extra points for completing this.)

Part 2: Scrape and Analyze Mars Weather Data
Open the Jupyter Notebook in the starter code folder named part_2_mars_weather.ipynb. You will work in this code as you follow the steps below to scrape and analyze Mars weather data.

Use automated browsing to visit the Mars Temperature Data SiteLinks to an external site.. Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.
Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.

Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:

id: the identification number of a single transmission from the Curiosity rover
terrestrial_date: the date on Earth
sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
ls: the solar longitude
month: the Martian month
min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
pressure: The atmospheric pressure at Curiosity's location
Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.
nalyze your dataset by using Pandas functions to answer the following questions:

How many months exist on Mars?  12 months
How many Martian (and not Earth) days worth of data exist in the scraped dataset?  1867
What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:   The coldest month was month 3 at -83.31°C.
The hottest month was month 8 at -68.38°C.

Find the average minimum daily temperature for all of the months.
Plot the results as a bar chart.
Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:  Month 6 has the lowest atmospheric pressure and month 9 has the highest atmospheric pressure on Mars

Find the average daily atmospheric pressure of all the months.
Plot the results as a bar chart.
About how many terrestrial (Earth) days exist in a Martian year? To answer this question:  There are 687 terrestrial earth days in a Martian year

Consider how many days elapse on Earth in the time that Mars circles the Sun once.
Visually estimate the result by plotting the daily minimum temperature.
Export the DataFrame to a CSV file.