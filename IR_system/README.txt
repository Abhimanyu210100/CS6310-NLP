This folder contains the additional files required for building a search engine application. Note that this code works for both Python 2 and Python 3. 

The following files have been added:
informationRetrieval.py and evaluation.py - Implement the corresponding tasks inside the functions in these files.

The following file has been updated:
main.py - The main module that contains the outline of the Search Engine. Do not change anything in this file.


To test your code, run main.py as before with the appropriate arguments.
Usage: main.py [-custom] [-dataset DATASET FOLDER] [-out_folder OUTPUT FOLDER]
               [-segmenter SEGMENTER TYPE (naive|punkt)] [-tokenizer TOKENIZER TYPE (naive|ptb)] 

**NOTE: Naive method has been removed from the code**

When the -custom flag is passed, the system will take a query from the user as input. For example:
> python main.py -custom
> Enter query below
> Papers on Aerodynamics
This will print the IDs of the five most relevant documents to the query to standard output.

When the flag is not passed, all the queries in the Cranfield dataset are considered and precision@k, recall@k, f-score@k, nDCG@k and the Mean Average Precision are computed.

In both the cases, *queries.txt files and *docs.txt files will be generated in the OUTPUT FOLDER after each stage of preprocessing of the documents and queries.
