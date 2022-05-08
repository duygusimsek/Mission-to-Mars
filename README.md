# Mission to Mars

## Overview

The purpose of this project was to create a script that scrapes web pages and gathers the latest information from the [Nasa Science Mars Exploration](https://mars.nasa.gov/) website about the red planet, Mars. 

For that purpose, to identify the HTML elements, Chrome Developer tools, automate a web browser and scrape the webpage Beautiful Soup/Splinter, store the data Mongo DB and display the data on a webpage Flask were used. 

## Result

### 1. Scraping Full-Resolution Mars Hemisphere Images and Titles
*  For that purpose, the Mars Hemisperes website was visited to view the hemisphere images. By using the Developer Tools, the proper elements of the page were inspected to scrape. 

* A list was created to hold the .jpg image URL string and title for each hemisphere image.

* To retrieve the full-resolution image URL and title for each hemisphere image a code was written. “For loop” was used to Loop through the full-resolution image URL and get the href.

* The full-resolution image URL string as the value for the img_url key that was stored in the dictionary that had been created inside the “for loop”.

* The hemisphere image title as the value for the title key that was stored in the same dictionary that had been created.[Mission_to_Mars_Challenge.ipynb](https://github.com/duygusimsek/Mission-to-Mars/blob/main/Mission_to_Mars_Challenge.ipynb)

* The list of dictionary items was printed. 
 
![hemisphere_image_urls](https://github.com/duygusimsek/Mission-to-Mars/blob/main/ScreenShots/hemisphere_image_urls.png) 



### 2. Updating the Web App with Mars Hemisphere Images and Titles

* The Jupiter notebook file that was created, was exported into a Python script. This script had been used as a starting point and to edit it VS Code was used to define the scraping progress. 

* Functions were created to scrape through the website and loop through the HTML tags to return the information used to create a database to be stored in MongoDB.

* In the def **scrape_all()** function in the [scraping.py](https://github.com/duygusimsek/Mission-to-Mars/blob/main/scraping.py) file, a new dictionary in the data dictionary was created to hold a list of dictionaries with the URL string and title of each hemisphere image.

* In the def **mars_facts()** function in the [scraping.py](https://github.com/duygusimsek/Mission-to-Mars/blob/main/scraping.py) file, a function that will scrape the hemisphere data was created. At the end of the function, the scraped data was retrieved as a list of dictionaries with the URL string and title of each hemisphere image by using the return function. ![Hemispheres_image_4.png](https://github.com/duygusimsek/Mission-to-Mars/blob/main/ScreenShots/Hemispheres_image_4.png)

* In the terminal, the [app.py](https://github.com/duygusimsek/Mission-to-Mars/blob/main/app.py) file was run, and the Mongo database was updated. 

* To access the database, the [index.html](https://github.com/duygusimsek/Mission-to-Mars/blob/main/templates/index.html) was modified. 

* To open the [index.html](https://github.com/duygusimsek/Mission-to-Mars/blob/main/templates/index.html) file with a click, the "Scrape New Data" button was created. 
* [The first view of webpage](https://github.com/duygusimsek/Mission-to-Mars/blob/main/ScreenShots/Screen%20Shot%202022-05-05%20at%2010.34.57%20PM.png)

### 3. Adding Bootstrap Components









## Resource 
* Crome Developer 
* VS Code
* Beautiful Soup/Splinter
* Mongo DB
* Flask 
* Jupiter Notebook 
