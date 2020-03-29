# Text-Adaptive Generative Adversarial Network alongwith BRL(TAGAN-BRL)
Part of our final year project where we built upon the existing TAGAN architecture to include better conditioning methods (of FiLM and Low Rank Bilinear Representation (BRL)) and also add BERT embeddings instead of pretrained FastText ones to include context. 

![Model architecture](images/architecture.png)

## Requirements
- [PyTorch](https://github.com/pytorch/pytorch) 1.0
- [torchfile](https://github.com/bshillingford/python-torchfile)
- [Visdom](https://github.com/facebookresearch/visdom)
- [Pillow](https://pillow.readthedocs.io/en/4.2.x/)
- [fastText](https://github.com/facebookresearch/fastText)
- [NLTK](http://www.nltk.org)

## Datasets
- Caltech-200 birds: [images](http://www.vision.caltech.edu/visipedia/CUB-200-2011.html) and [captions](https://drive.google.com/file/d/0B0ywwgffWnLLLUc2WHYzM0Q2eWc/view?usp=sharing)

The caption data is from [this repository](https://github.com/reedscot/icml2016). After downloading, modify `CONFIG` file so that all paths of the datasets point to the data you downloaded.


## Run  
Train a network. If you want to change arguments, please refer to `train.py`.
- `scripts/test_[flowers/birds].sh`  

