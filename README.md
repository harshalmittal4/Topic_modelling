# Topic_modelling
The repo contains code for topic modelling in python using LDA (latent dirichlet allocation) done as a part of intern assignment.

## Aim:
Given a csv file containg the following fields:
   1. ID,
   2. Job Role/Title, 
   3. Job Description and 
   4. Category ;
   
we have to extract skills (or important keywords) from each of the job titles; basically, in the dataframe, a new column is to be added which contains the important skills for the job described in the respective rows.

As an initial try, the model is trained on kaggle dataset Tweeets.csv in which the 'text' column represents the 'Job description' column for the original problem from which topics(skills) will be extracted.

## Steps :
### For each job description:
1)A corpus(list of documents) is created and it is cleaned using nltk (removing stopwords, punctuation, slang).
2)A dictionary is prepared from the corpus which is followed by preparation of a <i>document_term _matrix</i>.

<i>Document_term_matrix: Python list having length equal to number of documents; it contains the number of occurences of each word of the dictionary in a document.</i>

3)Then an LDA model is built which is given as input the corpus an d the number of topics into which it is supposed to categorize the corpus.
4)Each word of the corpus is assigned to one of the topics and for each topic we have a probability distribution over the words that are categorized under it. 
5)Output for a topic here is being taken as the most probable word under that topic; although we increase the number of words as output for some topic (the words categorized under that topic) with decreasing priorities.

### Number of topics for a job description :
It is taken as the length of corpus; and so we have those many words (skills) extracted for a particular job description.







