# Semantic-analysis

With the emergence of social media websites, platforms that provide microblogging experiences have experienced a large increase in the variety of viewpoints and portraits of thinking. With such a wide userbase and real-time sharing of opinions, updates, and trends, hate
speech, abuse, and bullying have increased significantly. As a result, the goal of this project is to detect hate speech remarks or comments across the site. This approach employs the larger notion of sentiment analysis, in which every view is classified as either positive or
negative, or neutral in some cases, depending on the context.

<img width="315" alt="Screen Shot 2023-05-12 at 12 56 40 PM" src="https://github.com/srirakshareddy/Semantic-analysis/assets/132956605/a8de85f6-fedd-4528-8576-7afb6a0588d7">

I have divided the project into two separate files to distinguish the TF-IDF and Bag of words approach, and the deep learning neural network (GRU) approach. 

**Dataset:**
1. nlp_final_data.csv : We have shared in the project folder.
2. glove.twitter.27B.200d :
https://www.kaggle.com/datasets/fullmetal26/glovetwitter27b100dtxt

Hate speech detection on twitter data needed an specific environment creation where our data processing and models would work optimally. I have applied a few models and then taken an approach to compare them in order to find the most suitable approach for the problem.
I added a custom set of stop words which are unique to this context, it helped remove unnecessary terms. 

**Data Preprocessing** state involved Stemming, tokenization and Lemmatization. 

**Model:** I have used a TF-IDF (Term Frequency- Inverse Document Frequency) method for text analysis to quantify terms for the first time. The system determines the words which are essential in this method. Here I have utilized the Scikit TF-IDF for this method. I am also using a CountVectorizer that converts a text into a vector based on the frequency (count) of each word that appears in the text. Along with this I am employing ngrams by producing a bag of words with range from 1 to n, This method is mostly used for creating various features by taking the words of a phrase, we have utilized 2000 features and the training data is 90506. The rationale behind this is if each phrase contains an average of 8 features, there will be a large number of features in the dataset that will be unsuitable for our processor because of which I have utilizing 2000 features, I have also used the Bag of words method to compare the difference in accuracy of the classifier algorithms.

**GRU (Gated Recurrent Unit)**: RNN (Recurrent Neural Network) is a type of network model that can handle sequence data, and it is needed by the designer to gather and reuse earlier knowledge. However, the research discovered that learning long-term information using a simple RNN was challenging, and issues like gradient expanding and gradient vanishing occurred often during the calculating process. Hence I improvised the RNN approach by considering a GRU (Gated Recurrent Unit). GRU with gated structure is another upgraded RNN model that includes Reset Gate and Update Gate. Filtering information and updating status is handled by the Update Gate. Furthermore, GRU combines cell state and hidden state, and the final output is not the same as RNN. I used GRU due to its great efficiency and simple structure and operation.

Overall, semantic analysis is a very fun exercise to explore the uses of Natural Language Processing.

Steps to be followed to run the code:
1. Make a environment for specific importing libraries
2. Install libraries as per requirements of project
3. Provide the path for accessing dataset
4. Restart and Run
