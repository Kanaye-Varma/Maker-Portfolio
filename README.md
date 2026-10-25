# Maker Portfolio

This is my Maker Portfolio submission. 

> [!IMPORTANT]
> I did not start this project expecting it to become a portfolio project. As a result, this repo is not fully version-controlled, and only the final version of each file has been uploaded. The attached write-up contains snippets of old code obtained from local history where appropriate, but it was not feasible to upload the full version history to GitHub. 

### What I made  
I have made an image-captioning model. It generates short, descriptive captions for input images. 

You can access a working demo [on this link](https://huggingface.co/spaces/kanaye/Portfolio). It is best used on a phone, where you can take and upload photographs. You can also choose to upload image files from your computer. 

Copy-paste this text into your browser if the link does not work: https://huggingface.co/spaces/kanaye/Portfolio

You may be prompted to restart the space if it has been inactive for a long time. Restarting will lead to it being re-built and will take some time to load. 

The files on Hugging Face include the actual model weights and a script that loads them. These are available to view if needed. 

### Evaluation 
> [!NOTE]
> Relevant file: `evaluate_it.ipynb`

This notebook is a detailed evaluation of the performance of the model over a large sample of images. These are validation images taken from the COCO 2017 dataset that the model has never seen before. The generated captions vary in quality. Some are quite detailed, some are satisfactory, some are hallucinatory, and some are outright nonsensical. You may use this to judge the quality of my model. 

A compressed pdf version of this file has also been uploaded to SlideRoom since this file is too large to preview on GitHub. It is 41 pages long and contains dozens of images. It is not meant to be read in detail, just skimmed through to get a rough idea of how the model performs on various images. 

### Word2Vec Embeddings 
> [!NOTE]
> Relevant file: `attempted_word2vec.ipynb`

This notebook shows my attempt to create Word2Vec embeddings. It shows the code used to generate these embeddings, as well as an evaluation over several words chosen by me to test the model's understanding of context. I have tried to feed the model diverse inputs to get a wide range of outputs of varying quality.  

### Data Generation And Training
> [!NOTE]
> Relevant file: `image_captioning_data_generation.ipynb`
> Relevant file: `training-image-captioning.ipynb`

These two notebooks were used for generating training data, as well as training the image captioning model. Note that the training notebook does not show the full training loop as training data for the first 3 epochs was lost. The first 3 epochs were trained using the same code but on a different notebook to get over GPU time constraints. 

Also note that there is a bug in the training image captioning noteboook. I accidentally hard-coded the scheduled sampling probability at 0.1. I did not fix this because by the time I noticed, I had already decided to discontinue the use of scheduled sampling instead of implementing it for all training epochs. This bug has had no effect on the actual training of the model. 
