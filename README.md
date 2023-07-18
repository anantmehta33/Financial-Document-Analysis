# Financial-Document-Analysis

The internship project involved working on natural language processing techniques. 
The first task was to successfully analyse the 'Financial Report Section' of the provided document.  
Named Entity Recognition tokens were extracted using four different libraries and the results were merged in one CSV file.
Code was written to automate the pipeline of reading a .pdf file and extracting the entities and making a new CSV containing the tokens. 
Second task involved making the financial section shorter by summarizing using extraction.
The third task was to build a QA system specific for the financial document. The client/investor can search for any information through the system. <br>

# Project 1: Required NER Extraction from Financial Document <br>
# Frameworks and Libraries used - NLTK, Flair, BERT, Spacy, PyPDF 2, fitz, NumPy <br>
# Description: <br>
The data from the all the libraries was taken collected and four different dataframes were created. 
Then these dataframes were merged into a single one using 'pd.concat()' function.\\
To do this first same entities were renamed under a single heading e.g., 'ORG' and 'ORGANIZATION' were put under one column 'org'. <br>

# Project 2: Document Summarization (Extractive) <br>
# Frameworks and Libraries used - NLTK, Spacy, base-BERT <br>
# Description: <br>
A concise information about the financial document was extracted using summa-
rization. Summarizers enable users to save time by swiftly obtaining a summa-
rized version of a document instead of reading it in its entirety. So, the process
of decision making is catalysed. <br>


# Project 3: A Q-A System based on the finanical Report <br>
# Frameworks and Libraries used - roBERTa-base fine-tuned on SQuAD v2.0 (hyperparameters tuned)<br>
# Description: <br>
All the sentences collectively are termed as ’context’. A context needs to be
fed in the pipeline along with the question. Reply is prompted by the model in a
json format, along with the first and last pointer location and confidence score
