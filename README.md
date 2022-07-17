# Natural Language Process Project

## Delivery-1

### Preprocessing

There are three steps to extract collocations
- Preprocessing
  - Removing stopwords
  - Stemming and Lemmatization
- Extracting the Bigrams and Trigrams
- Generating Collocations using related methods

### N-GRAM Frequencies

<img width="1226" alt="image" src="https://user-images.githubusercontent.com/33997918/179395427-fc72463d-8dc3-48d9-9a1d-deaf35578474.png">

### Methods

- **Raw Frequency**
- **PMI**
- **T-Test**
- **Chi-Square**
- **Likelihood Ratio**
- **Poisson Stirling**

### Raw Frequency Results

<img width="1162" alt="image" src="https://user-images.githubusercontent.com/33997918/179395728-398a1eff-fd8b-4178-b348-8260335b4c45.png">

### PMI Results

<img width="1195" alt="image" src="https://user-images.githubusercontent.com/33997918/179395850-c5a353d6-75d9-42c5-a556-208ab74c165e.png">

### T-Test Results

<img width="1195" alt="image" src="https://user-images.githubusercontent.com/33997918/179395891-457dbd18-7263-4564-ad5b-10dbda7e91ab.png">

### Chi-Square Results

<img width="1208" alt="image" src="https://user-images.githubusercontent.com/33997918/179395953-bde64473-c203-4399-afaf-f51e5840b907.png">

### Likelihood Ratio Results

<img width="1115" alt="image" src="https://user-images.githubusercontent.com/33997918/179395988-905ca0d3-6a31-4676-81b3-38004f792662.png">

### Poisson Stirling Results

<img width="1138" alt="image" src="https://user-images.githubusercontent.com/33997918/179396053-ff82205e-20b6-44d1-b10d-0eaca57f7095.png">

### Comparison of Methods

<img width="1199" alt="image" src="https://user-images.githubusercontent.com/33997918/179396124-ff29c7c8-c8b1-4d91-b388-982efb48884e.png">

<img width="1199" alt="image" src="https://user-images.githubusercontent.com/33997918/179396148-2a472890-c1a0-4b1f-89a0-9148baa1e0c2.png">

## Delivery-2

### Development Process

There are three steps to build a classifier for classification
- Preprocessing
  - Removing stopwords
  - Tokenization
  - Stemming
- Classifier
- Evaluation

### Preprocessing

- Dataset words converted to lowercase format
- Punctuation  marks from the dataset words are removed
- Tokenization process by using filtering options on the dataset words like extracting stopwords, applying some regex patterns
- Stemmization applied on the dataset words

### General Structure

- Files from dataset are read
- Labels created according to dataset
- Data.json file is created which holds labels we decided

<img width="675" alt="image" src="https://user-images.githubusercontent.com/33997918/179396563-047f5533-8430-41c6-8f55-d765426a8338.png">

### Generating Training Datasets

- Write data into CSV file
  - If there is no available train set created before, the csv file is created
- Read train set from CSV
  - If there is a previously created csv file that is available, the file is read. “Suç” and “İçtihat” are prepared as lists
- Split Dataset
  - Common approach is used for splitting the dataset which was 80% for training set and 20% for test set
- Vectorize
  - Using the data from our test set, a TF-IDF matrix is created

### Classifiers

- **Support Vector Machines (specifically, linear SVM)**
- **Multinomial Naive Bayes**
- **Logistic Regression**

### Support Vector Machine

<img width="1222" alt="image" src="https://user-images.githubusercontent.com/33997918/179397176-4de17648-7bb8-439c-aff7-34c7fe9b7921.png">

### Multinomial Naive Bayes

<img width="1222" alt="image" src="https://user-images.githubusercontent.com/33997918/179397223-b1b48cf4-6947-4db8-b8bc-0005dd909cef.png">

### Logistic Regression

<img width="1222" alt="image" src="https://user-images.githubusercontent.com/33997918/179397255-d771b429-23a0-4ba0-b2ae-f6170b4b0baa.png">

## Delivery-3

### Classifiers
- **FastText**
- **LSTM**

### FastText
- Dataset is taken from previous iteration
- Labels created according to dataset
- Label names concatenated with underscore to prevent ambiguity such as

<img width="927" alt="image" src="https://user-images.githubusercontent.com/33997918/179397536-1e0385fb-f3fc-4d77-8a56-f6a2ed6d0059.png">

- `__label__` tag is added to labels for model creation


## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="http://anilsenay.com"><img src="https://avatars.githubusercontent.com/u/1047345?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Anıl Şenay</b></sub></a><br /> <a href="https://github.com/anilsenay/CSE3063F20P1_GRP3/commits?author=anilsenay" title="Tests">⚠️</a> <a href="https://github.com/anilsenay/CSE3063F20P1_GRP3/commits?author=anilsenay" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/bilgehangecici"><img src="https://avatars.githubusercontent.com/u/33997918?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Bilgehan Geçici</b></sub></a><br /><a href="https://github.com/anilsenay/CSE3063F20P1_GRP3/commits?author=bilgehangecici" title="Tests">⚠️</a> <a href="https://github.com/anilsenay/CSE3063F20P1_GRP3/commits?author=bilgehangecici" title="Code">💻</a></td>
    <td align="center"><a href="http://www.linkedin.com/in/kursattacikgoz"><img src="https://avatars.githubusercontent.com/u/37029744?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Kürşat Açıkgöz</b></sub></a><br /><a href="https://github.com/anilsenay/CSE3063F20P1_GRP3/commits?author=kursatacikgoz" title="Tests">⚠️</a> <a href="https://github.com/anilsenay/CSE3063F20P1_GRP3/commits?author=kursatacikgoz" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/beyzaaydogan"><img src="https://avatars.githubusercontent.com/u/35075862?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Beyza</b></sub></a><br /><a href="https://github.com/anilsenay/CSE3063F20P1_GRP3/commits?author=beyzaaydogan" title="Tests">⚠️</a> <a href="https://github.com/anilsenay/CSE3063F20P1_GRP3/commits?author=beyzaaydogan" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/onkolahmet"><img src="https://avatars.githubusercontent.com/u/62245004?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ahmet Önkol</b></sub></a><br /><a href="https://github.com/anilsenay/CSE3063F20P1_GRP3/commits?author=onkolahmet" title="Tests">⚠️</a> <a href="https://github.com/anilsenay/CSE3063F20P1_GRP3/commits?author=onkolahmet" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/ElburuzGurbuz"><img src="https://avatars.githubusercontent.com/u/65295748?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ahmet Elburuz Gürbüz</b></sub></a><br /><a href="https://github.com/anilsenay/CSE3063F20P1_GRP3/commits?author=ElburuzGurbuz" title="Tests">⚠️</a> <a href="https://github.com/anilsenay/CSE3063F20P1_GRP3/commits?author=ElburuzGurbuz" title="Code">💻</a></td>
  </tr>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
