# IR2022_A2_37

# Preprocessing : #
For preprocessing, firstly we read the entire text files and remove all the \n, meaning we remove the next line and replace it with " " so that all the text is present in a single line. 
Then we put all the words into lower case
after that we remove all stop words from the text and tokenize the string.
We remove all special characters and digits and punctuation marks from tokens etc.
After all this you are left with tokens of preprocessed data in the form of lists and dictionaries.

# Methodology : #

Q1(a)
Imported folder as zip
Read all the documents
Preprocesses the data
Ask user for input query
Jaccard coefficient = intersect/union (between the query and document)
Sorted the documents based on decreasing values of jaccard coefficient
printed top 5 documents

Q2
Imported folder as zip
Read the data
Removed all the query-url pairs with qid != 4
Sorted the remaining lines based on the relevance score, for optimal ranking.
Lines with same score can be interchanged in order. That will not change the DCG.
Calculated nDCG at 50, and nDCG for the entire dataset
Created precision-recall curve for ranking based on feature 75.
