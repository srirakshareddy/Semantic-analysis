# Semantic-analysis

With the emergence of social media websites, platforms that provide microblogging experiences have experienced a large increase in the variety of viewpoints and portraits of thinking. With such a wide userbase and real-time sharing of opinions, updates, and trends, hate
speech, abuse, and bullying have increased significantly. As a result, the goal of this project is to detect hate speech remarks or comments across the site. This approach employs the larger notion of sentiment analysis, in which every view is classified as either positive or
negative, or neutral in some cases, depending on the context.

<img width="315" alt="Screen Shot 2023-05-12 at 12 56 40 PM" src="https://github.com/srirakshareddy/Semantic-analysis/assets/132956605/a8de85f6-fedd-4528-8576-7afb6a0588d7">

I am using the TF-IDF (Term Frequency- Inverse Document Frequency) method for text analysis to quantify terms for the first time. The system determines the words which are essential in this method. Furthermore, I am using the Scikit TF-IDF for this method and a CountVectorizer that converts a text into a vector based on the frequency (count) of each word that appears in the text. Along with this I am employing
ngrams by producing a bag of words with range from 1 to n, This method is mostly used for creating various features by taking the words of a phrase, I have utilized 2000 features and the training data is 90506. The rationale behind this is if each phrase contains an
average of 8 features, there will be a large number of features in the dataset that will be unsuitable for our processor because of which we are utilizing 2000 features. I have also used the Bag of words method to compare the difference in accuracy of the classifier algorithms.

From the experimental results, results are shown using the following metrics- precision, recall, f1-score, and accuracy. Although the comparison table is made of the TF-IDF methods with the accuracy. The Naive Bayes algorithm performed well in
terms of the time taken and testing accuracy. Moreover, the Stochastic Gradient Descent, SVM, and Logistic regression also showed almost similar accuracy. Besides, I have further explored the classification reports for four classifying algorithms where I used the Bag of
Words approach. In this approach, the Naive Bayes algorithms performed better than the other algorithms.

Overall, semantic analysis is a very fun exercise to explore the uses of Natural Language Processing.
