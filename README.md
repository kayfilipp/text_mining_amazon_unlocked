# Text Mining: Amazon Unlocked Phone Reviews
### Background:
The high level goal of this project is to:
<ol>
  <li>Ingest data using an API or Web Scraping tool</li>
  <li>Clean, tokenize, and otherwise normalize text data</li>
  <li>Linguistically process elements such as POS, NER, etc.</li>
  <li>Address class imbalances</li>
  <li>Create Feature vectors</li>
  <li>Train a model that can categorize reviews by rating</li>
  <li>Test the model against unseen data</li>
</ol>

<b>Dataset Background</b>
<p>The data used for this exercise is the Amazon Reviews dataset for unlocked mobile phones, which can be downloaded <a href="https://www.kaggle.com/datasets/PromptCloudHQ/amazon-reviews-unlocked-mobile-phones">here.</a></p>
<br>
Alternatively, the dataset can be loaded in directly with the Kaggle API, the documentation of which can be located <a href="https://www.kaggle.com/docs/api">here</a>.

```
pip install kaggle
kaggle.api.authenticate()
kaggle.api.dataset_download_files(
    'PromptCloudHQ/amazon-reviews-unlocked-mobile-phones', 
    unzip=True
)
```

### Navigating the Jupyter Notebook Space
Notebooks consist of distinct chunks of the data processing pipeline, divided into data preparation, ad-hoc foreign language removal, supervised learning for multi-class review modeling, supervised binary classification for sentiment analysis, and unsupervised topic modeling. 

![Slide1](https://user-images.githubusercontent.com/36943200/175841596-db21d037-b5e7-49b6-814d-a8691d759933.JPG)

