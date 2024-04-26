# Image Scraper & Dataset Organizer
This repository contains Python scripts for scraping image data from a website, organizing it into a DataFrame, downloading the images, and saving the dataset.

## Overview
The project consists of two main scripts:

#### 1. Scraping Images.ipynb: 
This script utilizes Selenium and BeautifulSoup to scrape image data from a specified website. It scrolls through the webpage to load all images, extracts relevant details such as image links, tags, likes, and comments, and saves the data into a pandas DataFrame. Finally, it removes duplicates and saves the DataFrame as a images.csv file.
#### 2. Downloading Dataset.ipynb: 
This script reads the previously saved CSV file containing image data, generates unique IDs for each image, downloads the images to a specified directory, and updates the DataFrame with image paths and IDs. It then saves the updated DataFrame as imgs2.csv file.

## Usage
- Execute the Scraping Images.ipynb script to scrape image data from the website and save it as images.csv file.
- Once the data is saved, execute the Downloading Dataset.ipynb script to download the images, generate IDs, and update the DataFrame.
- The final dataset will be saved as imgs2.csv, and the images will be downloaded to the specified directory.

## File Structure
- Scraping Images.ipynb: Jupyter Notebook containing code for scraping image data.
- Downloading Dataset.ipynb: Jupyter Notebook containing code for downloading images and updating the dataset.
- images.csv: CSV file containing raw scraped image data.
- imgs2.csv: CSV file containing updated image data with paths and IDs.

## Dependencies
- pandas
- tqdm
- requests
- beautifulsoup4
- selenium
- chromedriver-binary
