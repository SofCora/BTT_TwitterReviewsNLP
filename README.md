# BTT_TwtitterReviewsNLP
Classify book reviews as either positive or negative using a recurrent neural network **Deep Learning**

I chose  twitter sentiment analysis dataset from kaggle
These tweets are all about a product or service and I'm going to be classifying them as either positive or negative
This is a binary classification problem and there's no class imblanace.
Socil media is a good way to measure public reception of a new product so being able to parse out key words and determine the sentiment of the review would be key for companies to determine which products are popular and should be recommended to customers. For twitter this model will be useful to seeing what prodcuts users like and what ads should be shown to them.

· Describe the features that you will choose.
· Choose a model (or models) that you will train.
· Explain different data preparation techniques that you may use to prepare your data for your model.
· Specify an evaluation metric that you think is appropriate for your model.
· In your plan, describe your plan to train your model, analyze its performance and then improve the model. That is, describe your model building, validation and selection plan to produce a model that generalizes well to new data.
	There is only one feature in this dataset, which is the text of the review itself. I plan on using neural networks to determine the overall sentiment, ideally a recurrent neural network but I may run into issues with execution bottlenecks. Because I plan on using neural networks the reviews must be preprocessed before the feature-ization process where each document is compressed into a word embedding vector. The data preparation may include converting everything to lower case, removing stop words, stemming, and parsing it into smaller chunks. 
I'm going to be using AUC as the performance metric because it determines how well the predictions were regardless of their literal values and above any classification thresholds set.

Will try both feed forward networks and recurrent and if RNN's just aren;t working I can try downsampling and seeing if a downsampled RNN outperforms a feed forward network with a full dataset because i know a RNN will have better performance if i had comensurate computing power.
