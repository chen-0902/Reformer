# Reformer
* Reformer: the efficient transformer
* Category: NLP
* Topic: Transformers Efficiency Improvement

In this project, I explore the performance of the Reformer model on non-sequence-to-sequence tasks by comparing it with the original Transformer model on a sentiment analysis task. Utilizing the IMDB dataset, the models are trained and their accuracy and F1-score metrics are measured. Detailed information about the training and evaluation process can be found in the sentiment_analysis.ipynb notebook.

The results indicate that the Reformer model achieves performance similar to that of the original Transformer model on the sentiment analysis task. However, the Reformer model exhibits more fluctuation in training loss compared to the Transformer. This variability is likely due to the Reformer's use of locality-sensitive hashing for attention, which introduces approximations that can affect training stability.


## Experiment Results
|                        | Accuracy | F1-Score |  
|------------------------|:------:|:-----:|
| **Transformer**     | 0.7868 | 0.7930 | 
| **Reformer**          | 0.7709 | 0.7758 |

## Instruction to Run the Code
* `sentiment_analysis.ipynb` contains the code for training and evaluating the Transformer and Reformer models on the IMDB dataset. To run the code, you need to install the required packages: torch, torchtext, and reformer_pytorch.
* `inference.ipynb` contains the code for loading the trained models and making predictions on new text samples through a gradio interface. To run the code, you need to install the gradio package.
* `reformer_model_weights.pth` and `transformer_model_weights.pth` are the trained weights of the Reformer and Transformer models, respectively. You can load these weights to the models for inference. You can download from this link: https://drive.google.com/file/d/1vY6YuOrBfIoe6qHKjm9_F0XvLYnVrRp5/view?usp=sharing

## References
- Text classification with the torchtext library: https://pytorch.org/tutorials/beginner/text_sentiment_ngrams_tutorial.html
- reformer-pytorch: https://github.com/lucidrains/reformer-pytorch?tab=readme-ov-file
- IMDB dataset: https://ai.stanford.edu/~amaas/data/sentiment/




