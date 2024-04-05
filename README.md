## NLP final project on 'Unsupervised Lexical Simplification'
Submitted by Ayala Raanan
### 0. Read my paper
NLP_final_project_paper_git.pdf



### 1. Download sources

All of the data needed to run the project can be found at the shared google drive folder:

https://drive.google.com/drive/folders/1VWjQmdUnsvgbu0fbhtHfTdYcVqViqKzL?usp=sharing

To run in a local invironment, you need to download:

1. Fasttext embedding under: 'crawl-300d-2M.vec'
2. GloVe embedding under: 'glove.6B.300d.txt'
3. Word frequencies under: 'unigram_freq.csv'
4. 3 available datasets:
   - 'NNSeval.txt'
   - 'BenchLS.txt'
   - 'lexmturk.txt'

As results show, it is recommended to use Fasttext.

The code expects all resources to be under a folder './NLP_final_project/' (in root directory)

### 2. Run the code

All main functions of the code are provided in the following shared ipynb:

https://colab.research.google.com/drive/1bi6jqAqxUTZzhZMjc8WVuMWbzynhLsg_?usp=sharing

It contains all stages of processing:
- Stage 1. Embedding similarities
- Stage 2. POS and stem filtering
- Stage 3. Evaluating words in context using BERT

The code also saves intermediate calculations under './NLP_final_project/' and they can be loaded accordingly to skip stages of processing.

Function 'replace_word' at the very bottom allows one to play with free sentences and target words for replacement outside of the datasets.

It requires loading Fasttext and BERT (in the code) beforehand.
