# Text-Adaptive Generative Adversarial Network alongwith BRL(TAGAN-BRL)
Part of our final year project where we built upon the existing TAGAN architecture to include better conditioning methods (of FiLM and Low Rank Bilinear Representation (BRL)) and also add BERT embeddings instead of pretrained FastText ones to include context.

## Contribution
We have built upon existing TAGAN architecture. We used BRL layers which are proved to be effective to fuse image encodings and text embeddings. The text embeddings which were previously trained on Fasttext model were replaced with BERT to ensure contextual representation. Also moved the preprocessing code at runtime to ensure that memory is not overloaded and the code can work on machines with lower RAM. 

## Authors
- Fenil Doshi
- Parth Doshi
- Khushmann Dwivedi
- Jimit Gandhi
- Dr. Ram Mangrulkar (Supervisor)

## Requirements
- [PyTorch](https://github.com/pytorch/pytorch) 1.0
- [torchfile](https://github.com/bshillingford/python-torchfile)
- [Visdom](https://github.com/facebookresearch/visdom)
- [Pillow](https://pillow.readthedocs.io/en/4.2.x/)

## Datasets
- Caltech-200 birds: [images](http://www.vision.caltech.edu/visipedia/CUB-200-2011.html) and [captions](https://drive.google.com/file/d/0B0ywwgffWnLLLUc2WHYzM0Q2eWc/view?usp=sharing)

The caption data is from [this repository](https://github.com/reedscot/icml2016). 


## Run  
Train a network. If you want to change arguments, please refer to `train.py`.

