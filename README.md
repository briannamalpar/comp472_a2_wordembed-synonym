# comp472_a2_wordembed-synonym

Task 1: word2vec_google-news-300 Pre-Trained Model

Task 2: gigaword500-5th-edition & EngCoNLL17 

Task 3: Own word2vec model

# Stats
word2vec_google-news-300 ACCURACY: 0.8987

gigaword500-5th-edition ACCURACY: 0.7936

EngCoNLL17 ACCURACY: 0.7625

Own word2vec model ACCURACY:  Window size 5, Embedding size 100: 0.4259
                              Window size 10, Embedding size 100: 0.6101
                              Window size 10, Embedding size 300: 0.4339

Overall the word2vec pre-trained model performed the best with word classification, having an accuracy value of 0.8987. It was able to correctly guess the best synonym for all words except 8 (7 wrong , 1 guess). This is due to the fact word2vec is a huge corpus with vocab size of 300,000 and a large majority of the words found in synonym.csv were also found in word2vec and therefore proper cosine similarity can be performed. Gigaword500 and EngCoNLL17 performed similarly with classification and this can be due to the fact that even though EngCoNLL17 corpus has a very large vocabulary size of 4027169 (versus gigaword500' vocab size of 261,794) , the word embedding used is of size 100 therefore because of it's smaller size it has less capacity to learn complex relationships and patterns in the data. This is even more emphasized due to the fact that out dataset is very small and can lead to overfitting of data.

