# Final Project
## Network Judging Other Network's Album Art

Shawheen Tosifian, stosifia@ucsd.edu

## Abstract Proposal

This project is an extension of the Generative Visual project where a GAN was trained on 64x64 images of album covers and reproduced it's own 'album art'. This project extends on the concept by having an emotion 'classifer' network based of the pretrained VGG16 model trained on a small abstract art dataset (url) assign an emotion to a piece of GAN 'album art'. The primary motivation behind is to see if album art is emotive (and if it matches the album's desired response through its music) and to see if a neural network can try to classify the 'emotion' that another neural network might have produced with its art. This can be extended to much greater depths but that'd be somewhat foolish to do for a GAN trained on 64x64 album artwork and a classifier on an even smaller dataset of abstract art.


FIRST STEP: Write up a description (in the form of an abstract) of what you will revisit for your final project. This should be one paragraph clearly describing your concept and approach. What are your desired creative goals? How are you expanding on something we covered in the class? How will you present your work next Wednesday in the final project presentations? 

## Project Report

Upload your project report (4 pages) as a pdf with your repository, following this template: [google docs](https://drive.google.com/open?id=1mgIxwX1VseLyeM9uPSv5GJQgRWNFqtBZ0GKE9d4Qxww).

## Model/Data

Briefly describe the files that are included with your repository:
- abstract_64x64 : directory containing images of abstract art resized to 64x64 (with corresponding .csv containing
                   each images sentiment labels) obtained from https://www.imageemotion.org
- abstractclass1 : checkpoints for classifier
- dcgan_results : sample output of DCGAN over every iteration
- GANAlbumArt : contains generated DCGAN 'album art' files
- AbstractClassifier: .ipynb notebook for classifier
- DCGAN_AlbumArt: .ipynb notebook for DCGAN
- nntools.py: used by AbstractClassifier for importing classes/functions needed to run model
- README.md: where you are now

## Code

Your code for generating your project:
- Python: nntools.py <- needed to run AbstractClassifier.ipynb
- Jupyter notebooks: DCGAN_AlbumArt.ipynb <- train and generate 64x64 'album art'
                     AbstractClassifier.ipynb <- classifies 'album art' with emotion

## Results

Documentation of your results in an appropriate format, both links to files and a brief description of their contents:
- What you include here will very much depend on the format of your final project
-> In AbstractClassifier.ipynb for now


## Reference

References to any papers, techniques, repositories you used:
https://www.imageemotion.org
