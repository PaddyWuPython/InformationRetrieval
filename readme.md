# Project overview

__Optimization of text-based Search Engine__

## Intro to Datasets(from Assignment 1)

- FIR-s05-medline.json (the collection in Elasticsearch batch format - because of its size it cannot be indexed with a single curl command!)
- FIR-s05-training-queries-simple.txt (test queries)
- FIR-s05-training-qrels.txt (the "relevance judgements" for the test queries, i.e. the correct answers)

## Optimization direction

- Adjust the parameters of the search model and improve the design of the search model
- Optimize index configuration and improve index strategy

## Optimization strategy

- Optimize the parameters of the existing model
- Mixed Model Design
  - For example, you can use BM25 for preliminary recall and then use Dirichlet smoothing to re-rank the recall results.
  - Use different recall re-ranking models (Bi-encoder + Cross-encoder)
- Optimize tokenization strategies
	- N-gram
	- Stemmer

## Introduction of the files

- Codes: The code we used, the code is ran on Google Colab([link](https://colab.research.google.com/drive/1tWGM_No9kxFrKh1ZqzObkuNhTaFujnPg?usp=sharing)).
- Data: It includes some data related to our research.
- Models:  The Sentence-transformers models we fine tuned. Because of space limit, we didn't upload the fine-tuned models. But the process of fine-tune is indicated in __Codes__.
- Results: The document of search results.

This is an overview of our thinking progress. In detail, please see the project reports! 

Thanks to my teammates: [Ken Yeh](https://github.com/ypj0202) and [Kelly Huang](https://github.com/kelly40427), They also contribute a lot to the report.

