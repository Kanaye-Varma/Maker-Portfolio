# Maker Portfolio

This is my Maker Portfolio submission. 

> [!IMPORTANT]
> This was not initially meant to be a portfolio project. As a result, this repo is not fully version-controlled, and only the final version of each file has been uploaded. The attached write-up contains snippets of old code obtained from local history where appropriate, but it was not feasible to upload the full version history to GitHub. 

### What I made  
I have made an image-captioning model. It generates short, descriptive captions for input images. 

You can access a working demo [on this link](https://huggingface.co/spaces/kanaye/test). It is best used on a phone, where you can take and upload photographs. You can also choose to upload image files from your computer. 


### Write Up
> [!NOTE]
> Relevant file: `writeup.pdf`

This is a PDF write-up of the project. It explains the build process, challenges encountered, debugging methods, and reflections on what I learnt. It is meant to be the focus of this project. 


### References 
>[!NOTE]
> Relevant file: `references.pdf`

This file is a detailed, comprehensive citation of all external resources and materials that are not entirely my own work. It is to get over the 900 character limit so that my citations can be thorough and honest. 

### Evaluation 
> [!NOTE]
> Relevant file: `evaluate_it.ipynb`

This notebook is a detailed evaluation of the performance of the model over a large sample of images. These are validation images taken from the COCO 2017 dataset that the model has never seen before. The generated captions vary in quality. Some are quite detailed, some are satisfactory, some are hallucinatory, and some are outright nonsensical. You may use this to judge the quality of my model. 
### Word2Vec Embeddings 
> [!NOTE]
> Relevant file: `attempted_word2vec.ipynb`

This notebook shows my attempt to create Word2Vec embeddings. It shows the code used to generate these embeddings, as well as an evaluation over several words chosen by me to test the model's understanding of context. I have tried to feed the model diverse inputs to get a wide range of outputs of varying quality.  

### Data Generation And Training
> [!NOTE]
> Relevant file: `image_captioning_data_generation.ipynb`
> Relevant file: `training-image-captioning.ipynb`

These two notebooks were used for generating training data, as well as training the image captioning model. Note that the training notebook does not show the full training loop as training data for the first 3 epochs was lost (they were trained separately to get over GPU time constraints). Further context is provided in the notebook itself. 