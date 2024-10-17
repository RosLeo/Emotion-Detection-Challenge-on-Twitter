# Emotion-Detection-Challenge-on-Twitter

## Project Description
This project was carried out for the hackathon dedicated to the Milan Digital Week by Open Data Playground. The sentiment analysis task involves a multiclass classification of 4 emotions:

1. 😠 **Anger** (class 0)
2. 😂 **Joy** (class 1)
3. 😀 **Optimism** (class 2)
4. 😞 **Sadness** (class 3)

My approach was to use a voting classifier. The project is based on several stages, including text preprocessing, tokenization, and merging the results of various machine learning models. In the end, the system produces a final prediction saved in a CSV file.

## Key Features

1. **Data analysis**: Histograms to understand the distribution of words based on emotions.
2. **Data preprocessing**: Stopword removal, text normalization, lemmatization.
3. **Data augmentation**: Applied a data augmentation technique by creating new text using synonyms of words (removed due to worse performance).
4. **Embedding**: Tested embedding with TF-IDF, Word2Vec, and pre-trained BART (best performance with TF-IDF).
5. **Integration of multiple models**: Combines predictions from different models.
6. **Voting system**: Determines the final prediction based on the mode of labels predicted by individual classifiers.
