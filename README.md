# google_patents_parser
Extraction of names of patents, scraping of data, parsing

 # patent_landscaping.ipynb
First of all, it is necessary to collect names of patents and their links for future scraping and parsing. Patent landscaping is the process of finding patents related to a particular topic. To do that we are going to use Google Cloud and Big Query, Python, and Anaconda. You can read in detail about all the technical requirements here: (https://github.com/google/patents-public-data/tree/master/models/landscaping). For this code, you can skip TensorFlow and Keras part. For to run the landscaping code clone this repository.
 # scrape_google_patent_with_beautifulsoap.ipynb
The next step is to get all information from each patent page and save it. Here will be created a big database from where is possible to extract any feature that can be found on each page.  Required changes:
data = pd.read_excel("insert here the pass to the file that was created in the previous example")
In the end, we will get a CSV file with data.
#  parsing_data.ipynb
Use this code to parse the data. Change the path of data = pd.read_csv(“path”) to the file that was a result of the previous example. 
