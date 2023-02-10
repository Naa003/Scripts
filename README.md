# Scripts
## Overview
These scripts are used to pull information from Pubmed such as Journal Name, First Author Name, Date Paper was published and Paper Title.

## Setup
To setup these scripts you must have Jupyter Notebook installed. [Anaconda Navigator](https://docs.anaconda.com/anaconda/install/) is highly recommended for Jupyter Notebook installation but not required.

Make sure to copy the scripts into your 
### Your jupyter notebook must have these packages:
* [BeautifulSoup 4](https://www.geeksforgeeks.org/beautifulsoup-installation-python/)
* [Pandas](https://pandas.pydata.org/docs/getting_started/install.html)
* [numpy](https://numpy.org/install/)
* [lxml](https://pypi.org/project/lxml/)

If you do not have any of these packages then you must install them before running the scripts.


## Get an API key from Pubmed. Read ["How to obtain an API Key Through an NCBI Account"](https://support.nlm.nih.gov/knowledgebase/article/KA-05317/en-us).

## Editing the scripts
You must input your API key into the ```api_key = '&exampleAPiKey'``` variable to gain access to Pubmed API.
Change the variables that contain Paths to point the script toward the files you want it to read.

ie: default location variable is: ```location = os.listdir(r'Directory of files you want to read')```

I would change this to ```location = os.listdir(r'C:\Users\Natei\Desktop\folder_with_my_files')```

Do this for all paths that reference where your files are being read from.
Do this for all paths that reference where your resulting export files will be saved from.

## About the Files

### GetAuthorName.ipynb
Pulls the relevant first author name from Pubmed for each PMID.

### JournalNameFromPMID.ipynb
Pulls the relevant Journal that each PMID was published in.

#### PaperTitleFromPMID.ipynb
Pulls the title of each Paper from the given PMID.

### PublishDateFromPMID.ipynb
Pulls the date that each paper was published using the given PMID.

### BiolegendWebIDsRecent.ipynb
User provides Biolegend Catalog Numbers and is returned Biolegend WebIDs necessary for their data export.
