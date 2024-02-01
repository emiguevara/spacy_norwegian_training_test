# Spacy NB config files

Since V. 3, Spacy has included config.cfg files in their official packages.
We can use these files to adapt our training to the latest functionality in the official models.

I have harvested these example files from:
- https://github.com/explosion/spacy-models/releases/download/nb_core_news_sm-3.7.0/nb_core_news_sm-3.7.0.tar.gz
- https://github.com/explosion/spacy-models/releases/download/nb_core_news_md-3.7.0/nb_core_news_md-3.7.0.tar.gz
- https://github.com/explosion/spacy-models/releases/download/nb_core_news_lg-3.7.0/nb_core_news_lg-3.7.0.tar.gz

Generally:
- the sm model (without vectors) achieves about 0.75 NER-F1 score
- the md model (500k words/embeddings pruned to 20k in the model), goes up to 0.81 NER-F1
- the lg model (500k words/embeddings with no pruning), goes up to 0.85 NER-F1

The performance is clearly correlated to the number of vectors in the model.


