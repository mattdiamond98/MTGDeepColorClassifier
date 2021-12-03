# MTGColorClassifier

## Abstract

Trading card games are a unique design space because of the natural categorization that arises from designing similar cards. *Magic: the Gathering*'s color system is a deeply important element of the twenty-eight year old card game. By training a model to classify colors of *Magic* cards, one can gain insight into the patterns behind the game in a unique way. By using a pretrained transformer model for text embedding, combined with a traditional neural network, I propose a new method of classifying colors of *Magic* cards. This model opens up a new lens of analysis into the card game.

## Required Dependencies

numpy

pandas

itertools

matplotlib

torch

json

sklearn

transformers

## Datasets

Source: https://www.kaggle.com/mylesoneill/magic-the-gathering-cards

Required Files:

AllCards.json

SetList.json

## Code

The code is broken into two parts (I recommend using the notebooks if you want to try to reproduce).

The first file is MagicColorPreprocessing.ipynb. This converts the raw data into mtg_train_data.json and mtg_test_data.json. If not using Google Colaboratory, all of these paths will need to be changed.

The second file is MagicColorClassifier.ipynb. This is responsible for data loading, model architecture, model training, saving and loading versions of the model, and analysis on the output.

## Other files

I have included the files produced by these notebooks, specifically the preprocessed train/test split, and the pandas DataFrame output of the final model. These can be found in the lib folder. If running locally, I recommend changing all paths to load from and save to this folder. The model weights are too large to include but a link can be found:

https://drive.google.com/file/d/1-5TRYpvyXC_mJbA8C7ZDO39wa52ATdlD/view?usp=sharing

A copy of the paper is included in this repository as well: Multilabel_Classification_of_Trading_Card_Game.pdf