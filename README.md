# Coursework from Udacity Deep Learning
August 2018

---

This repo contains finished homework assignments from a [Deep Learning](https://classroom.udacity.com/courses/ud730) course on the Udacity platform.
There are 6 six assignments and a final project.
All task were done in Jupyter notebooks.
There were not reviewed by course instructors or peers.
The whole course is organized to use Tensorflow.

### Materials

##### Data
- [notmnist](http://yaroslavvb.blogspot.com/2011/09/notmnist-dataset.html) - a dataset of latin characters in various formats as images
- [text8](http://mattmahoney.net/dc/textdata) - a piece of English wikipedia's dump
- [svhn](http://ufldl.stanford.edu/housenumbers/) - street view house numbers dataset, a dataset of pictures with house number plates at original angles, sizes, lengths, etc.

##### Notebooks

1. **1_notmnist** focuses on downloading and unpacking, building a baseline logistic regression. Multi-class accuracy at 50k training set is 88.1%.
2. **2_fullyconnected** introduces a fully connected neural net with 1 hidden layer. It is trained with SGD for 10k steps with batch size 256 (i.e. 12.8 full runs over the training set) full runs on the 200k dataset. Accuracy slightly improves to 91% for 10k test set.
3. **3_regularization** talks about the problem of overfitting. L2-regularization and Dropout are used to fight this issue.
4. **4_convolutions** finally sheds light on convolutional nets. They further improve the overall performance on notmnist. The concepts of pooling, strides and padding are also put in practice. LeNet-5 architecture is used for final training.
5. **5_word2vec** takes it to the realm of recurrent neural networks. A word2vec model is trained as both skip-gram and cbow approaches on the Text8 data.
6. **6_lstm** switches to text generation on a character level using LSTM architecture. (not finished)
7. **LiveCameraApp_1** and **LiveCameraApp_2** are attempts to build a house number recognition model based on a deep convnet. They follow [Ian Goodfellow's paper](https://arxiv.org/abs/1312.6082). Accuracy on validation is a bit higher than 60%. A model uses 5-layer-deep convolutional blocks and 5 fully-connected output layers (one for each digit in a dataset). 
