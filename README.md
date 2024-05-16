# proco-take-home-assignment

## The provided code is Python scripts build in jupiter notebook for scraping data from the Franchise Supplier Network website. Here's a breakdown of the code functionalities:

## Features

- Scrapes supplier details from the FSN website.
- Extracts information from resource pages.
- Downloads images from supplier pages and resource pages.
- Downloads content from individual blogs.
- Generates Excel files with scraped data.
- Supports downloading of images for offline use.


## Prerequisites

Before running the scripts, ensure you have the following prerequisites installed:

- Python 3.x
- Required Python packages (specified in the script files)
- An internet connection
- Clone this repository to your local machine using Git
- Navigate to the project directory

## Home_Details.text

- This script extracts text content from the Home page of the website.
- It uses BeautifulSoup to parse the HTML content.
- It iterates through various sections like sliders, headings, and paragraphs.
- It extracts text content and image links associated with these sections.
- Finally, it saves the extracted content in a text file named "Home_Details.text".


## Home_Image_details/excel and download images

- This script focuses on images from the Home page.
- It extracts image URLs, alternative text (Alt text), and file names from the image elements.
- It creates a Pandas DataFrame containing these details (Category, File Names, Images, Links).
- It saves the DataFrame as an Excel file named "Home_Img_Details.xlsx".
- It iterates through the DataFrame and downloads the images to a designated folder.


## Home/Resource_details

- This script focus to target the "Resources" page of the website.
- It iterates through multiple pages (up to 16) using a loop.
- It extracts details like category, resource ID, image link, heading, and meta description for each resource.
There are two commented options:
- One to create an Excel file named "Home_Resource_Detials.xlsx" with the extracted data.
- Another to display the data as a DataFrame directly in the Jupyter notebook, including displaying the images.

## Home/Resource_image_downloads

- This script focuses on downloading images from the "Resources" page.
- It iterates through multiple pages (up to 16) using a loop.
- It extracts the image link for each resource.
- It downloads the image and saves it to a designated folder with the filename extracted from the URL.



## Home/Resource/Individual_Blogs

- This script targets individual blog posts from the "Resources" page.
- It iterates through a list of blog post URLs.
- For each blog post URL, it extracts the title, headings, and paragraphs using BeautifulSoup.
- It saves the extracted content for each blog post in a separate text file named after the blog post (likely using the URL).




## Home/fsn-suppliers

- This script focuses on the "FSN Suppliers" page.
- It iterates through multiple pages (up to 8) using a loop.
## It extracts various details for each supplier, including:
- Supplier name (from heading)
- Category
- Image link
- Supplier page link
- Alt text for the image
## It also fetches additional details from the individual supplier pages using the extracted links:
- Founded date
- Headquarters & Regions
- Description (if available)
## There are two commented options:
- One to create two separate Excel files (one for details and another for descriptions)
- Another to display the data as a DataFrame directly in the Jupyter notebook.



## Home/fsn-suppliers/image_downloader

- This script downloads images from the "FSN Suppliers" page.
- It iterates through multiple pages (up to 8) using a loop.
- It extracts image URLs for each supplier.
- It downloads the image and saves it to a designated folder with the filename extracted from the URL.


## Home/About

- This script extracts text content from the "About" page of the website.
- It uses BeautifulSoup to parse the HTML content.
- It extracts headings and paragraphs from different sections of the page.
- It combines the extracted content and saves it in a text file named "Home_About.text".

