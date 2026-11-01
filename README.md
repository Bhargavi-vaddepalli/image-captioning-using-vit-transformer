
# Image Captioning Using Vision Transformer and Transformer

## Project Overview
This project focuses on generating natural-language descriptions for images using deep learning.

It uses a Vision Transformer (ViT) as the image encoder and a Transformer decoder to generate captions based on the visual features.

## Objectives
- Extract meaningful visual features from images.
- Generate relevant natural-language captions.
- Understand the practical implementation of encoder-decoder Transformer architecture.
- Train and evaluate an image captioning model using PyTorch.

## Technologies Used
- Python
- PyTorch
- Vision Transformer (ViT)
- Transformer Decoder
- Hugging Face Transformers
- DistilBERT Tokenizer
- COCO 2014 Dataset
- NVIDIA CUDA GPU

## Model Architecture

1. **Encoder:** Vision Transformer extracts image features.
2. **Decoder:** Transformer generates captions using the image features and previously generated tokens.
3. **Tokenizer:** DistilBERT tokenizer converts captions into token IDs.

## Dataset
This project uses the COCO 2014 dataset.

The dataset is not included in this repository because of its large size.

Download the dataset from:
https://cocodataset.org/#download

Required files:
- train2014 images
- val2014 images
- captions_train2014.json
- captions_val2014.json

## Project Structure

```text
image-captioning-using-vit-transformer/
│
├── Image_captioning.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Installation

Install the required packages:

```bash
pip install -r requirements.txt
```

For GPU training, install a PyTorch version compatible with your CUDA environment.

## How to Run

1. Clone this repository.
2. Install the required dependencies.
3. Download and extract the COCO 2014 dataset.
4. Configure the dataset paths in the notebook.
5. Open `Image_captioning.ipynb`.
6. Select a GPU-enabled PyTorch kernel.
7. Run the notebook cells in order to train the model and generate image captions.

## Hardware

The model was developed using an NVIDIA RTX 5090 GPU through OxCapsule.

## Future Improvements

- Improve caption quality.
- Experiment with different model configurations.
- Optimize training performance.
- Evaluate generated captions using suitable evaluation metrics.

## Author

Developed as a deep learning project to explore image caption generation using Transformer architectures.
