# Language-Modeling-Fastai-v2

The only requirements for running the notebooks in this repository are [fastai v2](https://github.com/fastai/fastai2) and its dependencies. If you wish to also replicate the results of the original authors, then you also need [Keras](https://keras.io/).

The 0_get_wiki notebook shows how to download the Wikipedia corpous of your language of choice. Notice that this notebook relies on the nlputils script used in [piegu's fastai-v1 language modeling repository](https://github.com/piegu/language-models) - it contains a regular expression which filters characters in the title and must be updated if your language includes characters which are not Latin or Hebrew.

Then, you should run the three steps sequentially - first the Wikipedia language model pre-training notebook (1_lm_wiki), then the dataset language model fine-tuning notebook (2_lm_data_dedup), and finally the text classification notebook (3_cls_data_dedup). You can then inspect the results of the model, including the most confusing test cases and the prediction confusion matrix.

The notebooks for the original dataset (which includes data leakage and duplicates) and for the binary classification task are included under the "other_versions" folder.

The sentiment analysis dataset in Hebrew provided here under the "data" folder has been taken from the [Neural Sentiment Analyzer for Modern Hebrew](https://github.com/omilab/Neural-Sentiment-Analyzer-for-Modern-Hebrew) repository.
