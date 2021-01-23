# Bangladesh District Statistics Dataset from Bangladesh Bureau of Statistics - 2011 Census

Original PDF Source: [[bbs.gov.bd]](http://www.bbs.gov.bd/site/page/2888a55d-d686-4736-bad0-54b70462afda/District-Statistics)

# Introduction

In this project, we are trying to extract the PDF data and clean it to turn it into easily readable formats (such as CSV and JSON) to be used easily by everyone.

## Goals

- The main aim is to create a digitized version of the 2011 census data by BBS so that anyone can access it and analyze it. 
- Once the data is online and freely accessible by anyone, they can use it for any purpose they wish. 
- The type of data is very diverse, example: number of school in each upazila, tons of rice produced, average wage of manual workers. So, this data captures many different aspects of Bangladesh in that time. 
- The data can be used is various studies and can also be used in data visualizations. 
- In the future, this data can be compared and/or merged with other data sources, example: the next census, and that will reveal some insights about Bangladesh. 
- Another further task is to take the individual tables and merge them into a mega table, where there will be one row for each upazila, and many many columns, side by side, so that data about any upazila or zila can be easily read.

# Notebooks

1. [1_docx_parser.ipynb](https://github.com/yasserius/bd_district_statistics_dataset/blob/main/1_docx_parser.ipynb): The PDFs from BBS have been converted into docx files using Adobe Acrobat Pro, and in this notebook, the docx is opened and the paragraphs and tables are extracted, then saved in a pickle.

2. [2_understanding_content.ipynb](https://github.com/yasserius/bd_district_statistics_dataset/blob/main/2_understanding_content.ipynb): the pickles are explored to show the format of the table and paragraph blocks.

3. [3_cleaning_and_formatting.ipynb](https://github.com/yasserius/bd_district_statistics_dataset/blob/main/3_cleaning_and_formatting.ipynb): the extracted tables and paragraph blocks are further cleaned and processed, and finally the blocks are sorted into chapterwise format.

4. [4_generate_csv.ipynb](https://github.com/yasserius/bd_district_statistics_dataset/blob/main/4_generate_csv.ipynb): the cleaned tables are converted into CSV files using pandas.

# Data Folders

- [cleaned_CSVs](https://github.com/yasserius/bd_district_statistics_dataset/tree/main/cleaned_CSVs): Contains all extracted CSV files, with 64 folders, one for each district. But this data is not verified.

- [verified_CSVs](https://github.com/yasserius/bd_district_statistics_dataset/tree/main/verified_CSVs): Contains the verified CSV files, also with 64 folders, one for each district. This data was verified manually by different contributors.

- [docx](https://github.com/yasserius/bd_district_statistics_dataset/tree/main/docx): Contains all docx files for every district, converted from PDF using Adobe Acrobat Pro.

- [pickles](https://github.com/yasserius/bd_district_statistics_dataset/tree/main/pickles): Contains all pkl file, which contains the cleaned data containing the table and paragraph blocks in a chapterwise format.

# Contribute



You can volunteer and take part in the data cleaning process, mail me if interested: yasser.aziz94 [aaat] gmail dot com

## How to contribute

1. Manually check the CSV files in the "cleaned_CSVs" folder and look for mistakes. Read the [**How to Clean Guide**](https://github.com/yasserius/bd_district_statistics_dataset/blob/main/CONTRIBUTING.md).
2. Programatically improve the extraction process from the PDFs so that the cleaning process is made easier.
3. Use the data to find insights or make helpful projects with this data.

## How to coordinate with other team members

1. Check [this Google Sheet](https://docs.google.com/spreadsheets/d/1sgcQSvns_XJ0uNDnYtMWr0_tURglhERWE-gd2BellDY/edit#gid=0) and follow the instructions on top. Choose the zila you want to work with and verify the tables inside. Submit your cleaned and verified files with a pull request.
2. Mail me to ask anything: yasser.aziz94 [aaat] gmail dot com
3. Post on the "Issues" tab if you face a difficulty.

## How credit will be given

Once you fork, verify the data and send a pull request, your submission will be checked and merged. Then your name will show up in the github repo under "Contributors".
