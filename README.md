# obf_autman
Extracting notes from PDF

PDF needs to have the stucture of the example.pdf
Annotations, such as test and certain attributes can be extracted.
A full list is can be examined in file tags.
All tags follow generally the rule:

#key xxx #

where key is the attribute key and xxx is the data to be extracted


## Install

### 1. install conda
1. **Check you don't already have conda installed!**
    1. `which conda`
    1. **if you already have it installed, skip ahead to Create an Environment**

1. If you do not have conda install conda from [here](https://conda.io/miniconda.html)).

### 1. Create an environment
1. Update conda:
    `conda update conda`
1. Create the environment. Call it pdftotext and install python 3 (*hence the name*):
    `conda create -n geo`
1. Activate the enviroment:
    `conda activate pdftotext`
1. Install packages:
    `conda install xxx`
    * pdftotext
    * pandas
    * ipykernel
1. Install kernel in Jupyter Notebook
    `python -m install ipykernel --user --name pdftotext`

## Run

### 1. Start Jupyter Notebook
1. Start Jupyter Notebook:
    `jupyter notebook`
1. Choose *pdftotext* kernel

### 1. Modify variables
1. Change number of pages to process as well as the input and output path:
    ```
    path_in = 'path_to_pdf/test.pdf'
    path_out = 'path_to_csv/test.csv'
    max_pages = 1000
    ```
    
### 1. Run cells
1. Run cells in Jupyter notebook