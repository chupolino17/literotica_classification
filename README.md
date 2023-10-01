# Explicit text classification

This work describes an approach to classifying the text as belonging to the presented categories of porn. The DistilBERT model is taken as a basis and is further trained on the dataset of porn stories we have collected.

# Content
This repository consist of Jupyter Notebooks with an [explicit text classification](literotica_classification.ipynb), [baseline solution](baseline.ipynb) and [scrapping example](literotica_anal_srapping.ipynb).

# Results
Based on the results of experiments with baseline and DistilBERT , the following results were obtained:
| model               | accuracy | precision | recall |
|---------------------|----------|-----------|--------|
| baseline (word2vec) | 0.45     | 0.62      | 0.45   |
| distilBERT          | 0.68     | 0.68      | 0.68   |


From the presented metrics, it can be seen that complex dependencies are observed in the data, from which a simpler model coped noticeably worse than the model that uses DistilBERT. This is due to the fact that the Transformer architecture allows you to retrieve more complex dependencies from the text, thanks to the attention mechanism.