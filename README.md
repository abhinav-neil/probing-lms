# Probing Language Models for Linguistic Features

## Overview

This project explores the encoding of linguistic features, such as Part-of-Speech (PoS) and syntax, in the contextualized representations (embeddings) of language models. The goal is to understand how well different types of models capture and encode these features.

We compare recurrent models (LSTM) with attention-based transformer models (GPT2-medium, DistilGPT2, OPT, and RoBERTa) to examine their performance in encoding linguistic features. Additionally, we investigate the differences between masked language models (e.g., RoBERTa) and autoregressive models (e.g., GPT2 and LSTM) in capturing linguistic information. Furthermore, we evaluate the performance of GPT2 models on languages other than English, including French and Italian.

Two probing tasks, namely PoS probing and structural probing, are employed to assess the models' ability to capture linguistic features. Baselines and control tasks are used as benchmarks for comparison.

## Project Structure

The project repository contains the following files and directories:

- `probing_lms.ipynb`: Jupyter Notebook containing the main code, analyses, and results.
- `requirements.txt`: List of required Python libraries and their versions.
- `README.md`: This file, providing an overview of the project.

The project also includes the following directories:

- `data/`: Directory containing the treebank corpora datasets used for evaluation.
- `lstm/`: Directory containing the pretrained LSTM model weights and vocabulary.

## Usage

1. Clone the repository:

```
git clone https://github.com/your-username/language-model-probing.git
```

2. Install the required Python libraries:

```
pip install -r requirements.txt
```

3. Place the treebank corpora datasets in the `data/` directory.

4. Run the Jupyter Notebook `probing_lms.ipynb` to execute the code and analyze the results.

## References

Please consider citing the following papers if you find this project helpful:

- Alexis Conneau, German Kruszewski, Guillaume Lample, Loïc Barrault, and Marco Baroni. 2018. What you can cram into a single $&!#* vector: Probing sentence embeddings for linguistic properties.
- John Hewitt and Percy Liang. 2019. Designing and interpreting probes with control tasks.
- John Hewitt and Christopher D. Manning. 2019. A structural probe for finding syntax in word representations.
- Dieuwke Hupkes, Sara Veldhoen, and Willem Zuidema. 2018. Visualization and 'diagnostic classifiers' reveal how recurrent and recursive neural networks process hierarchical structure.
- Ian Tenney, Patrick Xia, Berlin Chen, Alex Wang, Adam Poliak, R. Thomas McCoy, Najoung Kim, Benjamin Van Durme, Samuel R. Bowman, Dipanjan Das, and Ellie Pavlick. 2019. What do you learn from context? Probing for sentence structure in contextualized word representations.
- Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N Gomez, Łukasz Kaiser, and Illia Polosukhin. 2017. Attention is all you need.
- Yinhan Liu, Myle Ott, Naman Goyal, Jingfei Du, Mandar Joshi, Danqi Chen, Omer Levy, Mike Lewis, Luke Zettlemoyer, and Veselin Stoyanov. 2019. Roberta: A robustly optimized bert pretraining approach.
- Alec Radford, Jeffrey Wu, Rewon Child, David Luan, Dario Amodei, and Ilya Sutskever. 2019. Language models are unsupervised multitask learners. OpenAI Blog, 1(8).