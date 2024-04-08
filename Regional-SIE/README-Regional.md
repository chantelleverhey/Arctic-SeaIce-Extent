# README

This sub-folder for a comparative time series plot(s) to look at regional sea-ice extent differences in the Arctic. All data were from the NOAA - NSIDC Sea-ice analysis data-set.

https://noaadata.apps.nsidc.org/NOAA/G02135/seaice_analysis/ 

The original sourcing of the files downloaded from the link above were provided in .xlsx and needed to be converted to UTF-8 .csv in order to be compatible with the Polar TEP platform. This meant that the embedded tabs in the excel file had to be separated and blank rows were removed. In order to get yearly extent - an additional column was added to each regional data-set outlining the annual sea-ice average, and was not a part of the original data-set. Hence the datasets in this repository folder - to access the already formatted files follow the 'To Access...." instructions below. 

## To Access the NOAA dataset remotely, here is the script to do so:

import requests
import os

# URL of the data directory
url = "https://noaadata.apps.nsidc.org/NOAA/G02135/seaice_analysis/"

# Function to download files from the URL
def download_files(url, file_names, download_path="."):
    for file_name in file_names:
        file_url = url + file_name
        file_path = os.path.join(download_path, file_name)
        print("Downloading", file_name, "...")
        response = requests.get(file_url)
        with open(file_path, 'wb') as f:
            f.write(response.content)
        print(file_name, "downloaded successfully!")

# List of file names to download 'file1.csv' & 'file2.csv' are placeholders for the datasets that 
file_names = [
    "file1.csv",
    "file2.csv",
    # Add more file names as needed
]

# Directory where files will be downloaded
download_path = "./data"

# Create the download directory if it doesn't exist
if not os.path.exists(download_path):
    os.makedirs(download_path)

# Download files
download_files(url, file_names, download_path)
