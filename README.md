# BTT_bookreviewsNLP
Classify book reviews as either positive or negative using a recurrent neural network 

1. List the data set you have chosen.
I chose the book review data set from our unit on neural networks and deep learning.
2. What will you be predicting?
I will be predicting whether or not the review is positive or negative.
3. Is this classification or regression problem? If this is a classification problem, is there class imbalance?
This is a binary classification problem and while the classes likely won’t be split 50/50 there won’t be a major imbalance with the negative class being less than 5% of the total dataset.
4. Explain why this is an important problem. In other words, how would a company create value with a model that predicts this label?
Book reviews are completely subjective and thus hard to quantify into a standard 5 star rating, being able to parse out key words and determine the sentiment of the review would be key for an ecommerce company to determine which books are popular and should be recommended to customers.
5. Create a project plan.
· Describe the features that you will choose.
· Choose a model (or models) that you will train.
· Explain different data preparation techniques that you may use to prepare your data for your model.
· Specify an evaluation metric that you think is appropriate for your model.
· In your plan, describe your plan to train your model, analyze its performance and then improve the model. That is, describe your model building, validation and selection plan to produce a model that generalizes well to new data.
	There is only one feature in this dataset, which is the text of the review itself. I plan on using neural networks to determine the overall sentiment, ideally a recurrent neural network but I may run into issues with execution bottlenecks. Because I plan on using neural networks the reviews must be preprocessed before the feature-ization process where each document is compressed into a word embedding vector. The data preparation may include converting everything to lower case, removing stop words, stemming, and parsing it into smaller chunks. 
	I believe measuring accuracy will be the best for this project because neither a false negative or false positive will have disastrous effects once the model is deployed.

Will try both feed forward networks and recurrent and if RNN's just aren;t working I can try downsampling and seeing if a downsampled RNN outperforms a feed forward network with a full dataset because i know a RNN will have better performance if i had comensurate computing power.
