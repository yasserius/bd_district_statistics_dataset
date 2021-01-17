# Bangladesh District Statistics Dataset from Bangladesh Bureau of Statistics - 2011 Census

## UNDER CONSTRUCTION

Original PDF Source: [[bbs.gov.bd]](http://www.bbs.gov.bd/site/page/2888a55d-d686-4736-bad0-54b70462afda/District-Statistics)

In this project, we are trying to extract the PDF data and clean it to turn it into easily readable formats (such as CSV and JSON) to be used easily by everyone.

# Notebooks

1. [1_docx_parser.ipynb](https://github.com/yasserius/bd_district_statistics_dataset/blob/main/1_docx_parser.ipynb): The PDFs from BBS have been converted into docx files using Adobe Acrobat Pro, and in this notebook, the docx is opened and the paragraphs and tables are extracted, then saved in a pickle.

2. [2_understanding_content.ipynb](https://github.com/yasserius/bd_district_statistics_dataset/blob/main/2_understanding_content.ipynb): the pickles are explored to show the format of the table and paragraph blocks.

3. [3_cleaning_and_formatting.ipynb](https://github.com/yasserius/bd_district_statistics_dataset/blob/main/3_cleaning_and_formatting.ipynb): the extracted tables and paragraph blocks are further cleaned and processed, and finally the blocks are sorted into chapterwise format.

4. [4_generate_csv.ipynb](https://github.com/yasserius/bd_district_statistics_dataset/blob/main/4_generate_csv.ipynb): the cleaned tables are converted into CSV files using pandas.

# Data Folders

- [CSVs](https://github.com/yasserius/bd_district_statistics_dataset/tree/main/CSVs): Contains all CSV files, with 64 folders for every districts.

- [docx](https://github.com/yasserius/bd_district_statistics_dataset/tree/main/docx): Contains all docx files for every district, converted from PDF using Adobe Acrobat Pro.

- [pickles](https://github.com/yasserius/bd_district_statistics_dataset/tree/main/pickles): Contains all pkl file, which contains the cleaned data containing the table and paragraph blocks in a chapterwise format.

# Contribute

You can volunteer and take part in the data cleaning process, mail me if interested: yasser.aziz94 [aaat] gmail dot com
