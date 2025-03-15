# AI-vs-Human-Generated-Images-Deepfake-Detection
This project was part of a kaggle competition focused on distinguishing AI-generated images from human-created ones.


This is a concise and professional README for your Kaggle competition project:


---


## Project Overview

With the rise of generative AI, distinguishing between human-created and AI-generated images has become a crucial challenge. Deepfake detection is essential for maintaining media integrity, preventing misinformation, and ensuring security. This project involves training a machine learning model to classify images as either AI-generated or human-created using deep learning techniques.   

This project was submitted as part of the Kaggle AI vs Human-Generated Images Competition, where models were evaluated based on the F1-score at a 0.5 threshold.   

#### Competition Rank: 283/554   
#### F1-Score: 0.63359   

## Dataset   

The dataset consists of 79,950 training images and 19,986 test images, with labels indicating whether an image is AI-generated (1) or human-created (0).   

## Files:   

train.csv - Training set with image IDs and labels.   

test.csv - Test set with image IDs (labels are to be predicted).  

train_data/ - Folder containing training images.   

test_data/ - Folder containing test images.   


## Approach & Model   

### 1. Data Preparation:   

Split data into train and validation sets.   

Defined data augmentation techniques for training images.   

Created a custom dataset class for PyTorch.   



### 2. Model Selection & Training:   

Used EfficientNet-B3 as the base model (without pretrained weights).   

Set up train transforms and validation/test transforms for image preprocessing.   

Stopped training at Epoch 4 due to CPU limitations (initial plan: 12 epochs).   




## Future Improvements   

🚀 Train on GPU to allow for more epochs (20+ for better generalization).   
🚀 Experiment with pretrained models to enhance performance.   
🚀 Fine-tune hyperparameters to improve the F1-score.   

## Technologies Used   

Deep Learning Frameworks: PyTorch, Torchvision   

Model: EfficientNet-B3   

Data Handling: Pandas, NumPy   

Visualization: Matplotlib, Seaborn   


## Key Takeaways   

✅ Tackled a real-world deepfake detection challenge.   
✅ Implemented data augmentation and a custom dataset class.   
✅ Trained an EfficientNet-B3 model for classification.   
✅ Achieved an F1-score of 0.63359 on Kaggle.   

