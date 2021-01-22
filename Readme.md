# IBM Data Scinece Capstone

Indian restaurants have come a long way from the mid-1960's when the first significant wave of immigrants arrived. While still not entirely as assimilated as Italian and Mexican, Indian food is one of the fastest-growing segments in the culinary scene and is gaining popularity within the American mainstream. And as Indians have spread throughout America, so has their food. Restaurants with cult-like followings are no longer limited to New York City.

### Business Problem
Concerning the growing demand for Indian food and restaurants across the United States, the need for intelligent business solutions regarding opening Indian restaurants arises. For this project, we assume that a client in the city of San Diego wants to open an Indian restaurant. To maximize revenue and business success, insights into existing Indian restaurants and peer competition are required. Thus, the project's main objective is to find ideal spots in the city where Indian restaurants can be set up.

### Data
The data of the neighborhoods in San Diego can be extracted out by web scraping using the BeautifulSoup library for Python. The neighborhood data is scraped from a Wikipedia webpage:
https://en.wikipedia.org/wiki/Category:Neighborhoods_in_San_Diego

### Geocoding
The file contents from San-Diego.csv is retrieved into a Pandas DataFrame. The latitude and longitude of the neighborhoods are retrieved using the geocoder API. The geometric location values are then stored in the initial DataFrame.

### Venues
From the location data obtained after Web Scraping and Geocoding, the venue data is found out by passing in the required parameters to the FourSquare API, and creating another DataFrame to contain all the venue details along with the respective neighborhoods.

### Folium
Folium builds on the Python ecosystem's data wrangling strengths and the mapping strengths of the leaflet.js library. All cluster visualization is done with Folium's help, which generates a Leaflet map made using OpenStreetMap technology. 
Creating a map of San Diego with neighborhoods superimposed on top:
![Neighbourhoods in San Diego](https://github.com/divyaprakash0426/IBM_DataSciece-Capstone/blob/main/maps/map_sandiego.png)
