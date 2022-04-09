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

Q1(b)
binary:
  pro:useful because it is easy to understand and direct since either the score will be 1 or 0.
  con: will not take into consideration outlying data and hence a lot of data can be lost or result might not be precise.
raw count: 
  pro: Most basic and understandable form of tf yet the most used.
  con: can be far too basic if the data is needed for further statistics.
term frequency: 
  pro: term frequency is adjusted for document length therefore the value would be very accurate for each document.
  con: outlying data can cause a huge change in the overall mean data thus reducing accuracy.
log normalization: 
  pro:  Such a scale is nonlinear: the numbers 10 and 20, and 60 and 70, are not the same distance apart on a log scale. Rather, the numbers 10 and 100, and 60 and 600 are equally spaced.
  con: difficult to understand
double normalization:
pro: useful for augmented frequency, to prevent a bias towards longer documents, e.g. raw frequency divided by the raw frequency of the most frequently occurring term in the document(wikipedia)
con: dependable on document frequency of a different word and thus not accurate.
Imported folder as zip
Read the data
Removed all the query-url pairs with qid != 4
Sorted the remaining lines based on the relevance score, for optimal ranking.
Lines with same score can be interchanged in order. That will not change the DCG.
Calculated nDCG at 50, and nDCG for the entire dataset
Created precision-recall curve for ranking based on feature 75.
