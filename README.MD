# wordlab

The file BSOUP_WORDLAB_CITATIONS.ipynb is python code to scrape details from Urbanisation articles published on the Sage website. This code requires an input file "Urbanisation DOI list_edit.csv" with a list of website links to process. The code creates an output file "urbanisation_author_and_citation_detail.csv" with scraped details for each of the input links.

## Installations

Requires BeautifulSoup and selenium to be installed on your system.
Install geckodriver.exe and update the Path system variable to add the full directory path to the geckodriver.exe

## Usage

1. Download the .ipynb file to a folder on your system.
2. Input file "Urbanisation DOI list_edit.csv" must be available in the same folder as the .ipynb file
3. Output file "urbanisation_author_and_citation_detail.csv" with scraped details is created in the append (or update) mode in same folder as the .ipynb file when you execute the code

Note: If the code takes a long time to run, it may stop executing in between and not process all of the input records. From the print statements in the code find out which was the last record processed. Edit the input file to process from the next record onwards. Since the output file is used in the append mode, it will keep adding the new records but will also add the column header each time. Once all input records are processed delete the extra column header records from the output file. Rename the output file to reflect the month in which it was processed, for example, if you run the process in April 2022, rename the output file as "urbanisation_author_and_citation_detail_april_22.csv". 
