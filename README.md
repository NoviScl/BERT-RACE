# BERT for RACE

By: Chenglei Si (River Valley High School)

### Implementation
This work is based on Pytorch implementation of BERT (https://github.com/huggingface/pytorch-pretrained-BERT). I did some modification so that it can work on multiple choice machine comprehension.

### Environment:
The code is tested with Python3.6 and Pytorch 1.0.0.

### Usage
1. Download the dataset and unzip it. The default dataset directory is ./RACE
2. Run ```./run.sh```

### Hyperparameters
I did some tuning and find the following hyperparameters to work reasonally well:

BERT_base: batch size: 32, learning rate: 5e-5, training epoch: 3

BERT_large: batch size: 4, learning rate: 1e-5 (DO NOT SET IT TOO LARGE), training epoch: 2

### Results






