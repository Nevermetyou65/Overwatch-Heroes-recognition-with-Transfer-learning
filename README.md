# Overwatch-Heroes-recognition-with-Transfer-learning (with Xception)
Hello again visitors!:blush: This repository is my 5th hobby project about Data sciecne and Machine learning.This time I built DNN (Deep Neural Network) to predict "Which overwatch hero is that".

![alt text](https://www.mescript.com/upload/post/0/128/128-1-overwatch-review.webp)

## About overwatch :video_game:
For those of you who has not experience this overwatch, it is a MOBA-FPS online game by Blizzard Entertainment that features 32 playable character (heroes) at the time I writting this README.md

## About Dataset :file_folder:
Originally, the inspriation of me doing this small (but took me for a week to finish) project is that recently I found this dataset published on Kaggle ([here](https://www.kaggle.com/renanmav/overwatch-heroes-recognition)). SO, I take this oppotunity to get familiar with **TensorFlow** (a machine learning and deep learning framework by google written in python) and other aspect of the pipeling such as input data pipeline, tf.data and transfer learning etc.

This dataset was published 2 years ago and that means it does not contain some of new heroes. Because of that, I decided to collect more images of all heroes (both existed and not) and experience myself in the aspect of **"quality of data"**
I use these keywords to search for additionalimages
- Overwatch [hero name] 
- Overwatch [hero name] skins
- Overwatch [hero name] fanart
- (Sometimes) Overwatch [hero name] waepon <br>

But as I quite busy myself, I could not collect a signigicant amout of images, but still the data I used is more than the one in Kaggle repository.
Here is the URL to my images dataset directory ---->>> [DATA](https://drive.google.com/drive/folders/1FRpKK73Tk2fzPzlEgTo5qlDbYtlKOXOH?usp=sharing) if you are interested.

## About model
Because there are a smalle number of images in the dataset, It is a good time to try **"Transfer learning"** which is the ***pre-trained DNN***(you can think of it like someone who used to play tennis and he/she get familiar with badminton so easily) and build some of layers on top of it. In this case, I use **Xception** which is (if I am not mistaken) the start-of-the-art CNN for variety of image-relatied task developed by Google researcher and avalible in TensorFlow. There is an article that states this model has out-performed its predecessor like ResNet or Inception.

## The Result:sparkles:
The process of my project is like this
- build and check input image pipline
- training (back to previous if not good enough)
- fine tuning
- test on random images on internet

At the end after I finished fine-tuning my model, I managed to get **85% categorical accuracy** on validation datset which is quite impressive for a noob like me. You can see the result in jupyyer notebook file in this repository. But I have to note that my dataset is quite straightforward, meaning that my model is quite good on a not-very-fancy image. To make this clear, if you let my model try a **"female genji" pic** (which is too fancy because normal genji is a male-looking cyborg ninja) it will output other female hero instead. To fix this, I guess I need to collect more variation aspect of one hero.





