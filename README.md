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
Alternatively, the dataset can be loaded in directly with the Kaggle API.

```
pip install kaggle
kaggle.api.authenticate()
kaggle.api.dataset_download_files(
    'PromptCloudHQ/amazon-reviews-unlocked-mobile-phones', 
    unzip=True
)
```
