# Language-Modeling-Fastai-v2

The only requirements for running this repository are fastai v2 and its dependencies.

You should first run the get_wiki notebook in order to download the Wikipedia corpous of your language of choice. Notice that the nlputils script contains a regular expression which must be updated if your language includes characters which are not Latin or Hebrew.

Then, you should run the forward model notebook in three parts - first the Wikipedia language model pretraining, then the dataset language model pretraining, and finally the text classification task. You can then inspect the results of the model, including the most confusing test cases and the prediction confusion matrix.

Optionally, you can also train a backward model and then ensemble them to potentially obtain even better results
