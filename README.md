# Language-Modeling-Fastai-v2

The only requirements for running the notebooks in this repository are [fastai v2](https://github.com/fastai/fastai2) and its dependencies. If you also wish to replicate the results of the original authors, then you also need Keras.

You should first run the get_wiki notebook in order to download the Wikipedia corpous of your language of choice. Notice that the nlputils script contains a regular expression which must be updated if your language includes characters which are not Latin or Hebrew.

Then, you should run the forward model notebook in three parts - first the Wikipedia language model pretraining, then the dataset language model pretraining, and finally the text classification task. You can then inspect the results of the model, including the most confusing test cases and the prediction confusion matrix.

Optionally, you can also train a backward model and then ensemble them to potentially obtain even better results - check out the relevant notebook.

The sentiment analysis dataset in Hebrew provided here has been taken from the [Neural Sentiment Analyzer for Modern Hebrew](https://github.com/omilab/Neural-Sentiment-Analyzer-for-Modern-Hebrew) repository.
