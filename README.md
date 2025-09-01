# Reproducing-BERT-from-Scratch-with-PyTorch

I’m not the first to do this.  But it is something I must  do to clear up a lot of “gaps” in my head about how exactly **BERT (Bidirectional Encoder Representations from Transformers)**  is built.  I hope it does for you too.  It feels good to know where exactly all the nuts and bolts go and be able to comfortably say “there’s no magic”.  This is not to discount the magic of all the great people who created this.  This is for me and hopefully for you to deeply understand what BERT really is. 

### Repository Structure
`1. Data for BERT.ipynb`  
Processes the data to be compatible with BERT’s training objectives, including: 
* **Masked Language Modeling (MLM)**: randomly masks tokens in the input for prediction.
* **Next Sentence Prediction (NSP)**: constructs paired sentences (positive and negative examples).

`2. Reproducing BERT Model from Scratch using PyTorch.ipynb`  
Builds the BERT model architecture step by step in PyTorch and covers the main building blocks:
* **BERT Embeddings**: positional, token, and segment embeddings.
* **Transformer Blocks**: multi-head-attention and feed-forward layers
* **Output Layer**: MLM output and NSP output 

### Project Goals
* Gain a deep understanding of BERT by implementing it from scratch.
* Explore how data is prepared for masked language modeling and next sentence prediction.
* Learn the internals of Transformer blocks that power modern NLP models.

### References
* Devlin, Jacob, et al. "[Bert: Pre-training of deep bidirectional transformers for language understanding.](https://arxiv.org/abs/1810.04805)" Proceedings of the 2019 conference of the North American chapter of the association for computational linguistics: human language technologies, volume 1 (long and short papers). 2019. 
* Vaswani, Ashish, et al. "[Attention is all you need.](https://arxiv.org/abs/1706.03762)" Advances in neural information processing systems 30 (2017). 
* Adrian Tam. [Linear Layers and Activation Functions in Transformer Models.](https://machinelearningmastery.com/linear-layers-and-activation-functions-in-transformer-models/) 2025

### License  
This project is licensed under the MIT License.

