# Mission to Mars

## Overview

The purpose of this project was to create a script that scrapes web pages and gathers the latest information from the [Nasa Science Mars Exploration](https://mars.nasa.gov/) website about the red planet, Mars. 

For that purpose, to identify the HTML elements, Chrome Developer tools, automate a web browser and scrape the webpage Beautiful Soup/Splinter, store the data Mongo DB and display the data on a webpage Flask were used. 

## Result

### Scraping Full-Resolution Mars Hemisphere Images and Titles
*  For that purpose, the Mars Hemisperes website was visited to view the hemisphere images. By using the Developer Tools, the proper elements of the page were inspected to scrape. 

* A list was created to hold the .jpg image URL string and title for each hemisphere image.

* To retrieve the full-resolution image URL and title for each hemisphere image a code was written. “For loop” was used to Loop through the full-resolution image URL and get the href.

* The full-resolution image URL string as the value for the img_url key that was stored in the dictionary that had been created inside the “for loop”.

* The hemisphere image title as the value for the title key that was stored in the same dictionary that had been created.[Mission_to_Mars_Challenge.ipynb](https://github.com/duygusimsek/Mission-to-Mars/blob/main/Mission_to_Mars_Challenge.ipynb)

* The list of dictionary items was printed. 
 
![hemisphere_image_urls](https://github.com/duygusimsek/Mission-to-Mars/blob/main/ScreenShots/hemisphere_image_urls.png) 



### Updating the Web App with Mars Hemisphere Images and Titles



### Adding Bootstrap Components









## Resource 
* Crome Developer 
* VS Code
* Beautiful Soup/Splinter
* Mongo DB
* Flask 
* Jupiter Notebook 
