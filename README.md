# Topic_modelling
The repo contains code for topic modelling in python using LDA (latent dirichlet allocation) done as a part of intern assignment.

## Aim:
Given a csv file containg the following fields:
   1. ID,
   2. Job Role/Title, 
   3. Job Description and 
   4. Category ;
we have to extract skills (or important keywords) from each of the job descriptions and/or job titles.
So, in the dataframe a new column is added which contains the important skills for the job described in the respective rows.

## Steps :
For each job description, a corpus(list of documents) is created and it is cleaned using nltk (removing stopwords, punctuation, slang).
A dictionary is than prepared from the corpus which is followed by preparation of a document_term _matrix.




