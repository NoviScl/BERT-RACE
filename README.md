# BERT for RACE

By: Chenglei Si (River Valley High School)

### Update:
XLNet has achieved impressive gains on RACE recently. You may refer to my other repo: https://github.com/NoviScl/XLNet_DREAM to see how to use XLNet for multiple-choice machine comprehension problems. Huggingface has updated their work [pytorch_trainsformers](https://github.com/huggingface/pytorch-transformers), please refer to their repo for the documentation and more details of the new version. 

### Implementation
This work is based on Pytorch implementation of BERT (https://github.com/huggingface/pytorch-pretrained-BERT). I adapted the original BERT model to work on multiple choice machine comprehension.

### Environment:
The code is tested with Python3.6 and Pytorch 1.0.0.

### Usage
1. Download the dataset and unzip it. The default dataset directory is ./RACE
2. Run ```./run.sh```

### Hyperparameters
I did some tuning and find the following hyperparameters to work reasonally well:

BERT_base: batch size: 32, learning rate: 5e-5, training epoch: 3

BERT_large: batch size: 8, learning rate: 1e-5 (DO NOT SET IT TOO LARGE), training epoch: 2

### Results
Model | RACE | RACE-M | RACE-H 
--- | --- | --- | --- |
BERT_base | 65.0 | 71.7 | 62.3 
BERT_large | 67.9 | 75.6 | 64.7

You can compare them with other results on the [leaderboard](http://www.qizhexie.com/data/RACE_leaderboard).

BERT large achieves the current (Jan 2019) best result. Looking forward to new models that can beat BERT!

### More Details
I have written a short [report](./BERT_RACE.pdf) in this repo describing the details.




