# COMP 7404 Group Project

## Group 5 Members
* Feng Chenchen (group coordinator) u3612248@connect.hku.hk
* Li Xiaolong xia01ong@connect.hku.hk
* Tu Yuxi u3621409@connect.hku.hk
* Wang Yiyao yiyao258@connect.hku.hk

## Project Description
* Paper Title: Reformer: The Efficient Transformer
* Category: NLP
* Topic: Transformers Efficiency Improvement

In this project, we explore the performance of the Reformer model on non-sequence-to-sequence tasks. We compare the Reformer model with the original Transformer model on a sentiment analysis task. Specifically, we use the IMDB dataset to train and measure the accuracy and F1-score metrics. The detailed of the training and evaluation process can be found in the sentiment_analysis.ipynb notebook.

Based on the results, we observed that the Reformer model can achieve similar performance as the original Transformer model on the sentiment analysis task. However, the Reformer model exhibits more fluctuation in training loss compared to the Transformer. This variability is likely due to the Reformer's use of locality-sensitive hashing for attention, which introduces approximations that can affect training stability.

## Experiment Results
|                        | Accuracy | F1-Score |  
|------------------------|:------:|:-----:|
| **Transformer**     | 0.7884 | 0.7730 | 
| **Reformer**          | 0.7808 | 0.7870 |

## References
- Text classification with the torchtext library: https://pytorch.org/tutorials/beginner/text_sentiment_ngrams_tutorial.html
- reformer-pytorch: https://github.com/lucidrains/reformer-pytorch?tab=readme-ov-file
- IMDB dataset: https://ai.stanford.edu/~amaas/data/sentiment/



