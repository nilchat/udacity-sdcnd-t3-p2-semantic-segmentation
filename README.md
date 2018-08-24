# Semantic Segmentation
### Introduction
In this project, you'll label the pixels of a road in images using a Fully Convolutional Network (FCN).

### Setup
##### GPU
`main.py` will check to make sure you are using GPU - if you don't have a GPU on your system, you can use AWS or another cloud computing platform.
##### Frameworks and Packages
Make sure you have the following is installed:
 - [Python 3](https://www.python.org/)
 - [TensorFlow](https://www.tensorflow.org/)
 - [NumPy](http://www.numpy.org/)
 - [SciPy](https://www.scipy.org/)
##### Dataset
Download the [Kitti Road dataset](http://www.cvlibs.net/datasets/kitti/eval_road.php) from [here](http://www.cvlibs.net/download.php?file=data_road.zip).  Extract the dataset in the `data` folder.  This will create the folder `data_road` with all the training a test images.

### Start
##### Implement
Implement the code in the `main.py` module indicated by the "TODO" comments.
The comments indicated with "OPTIONAL" tag are not required to complete.
##### Run
Run the following command to run the project:
```
python main.py
```
**Note** If running this in Jupyter Notebook system messages, such as those regarding test status, may appear in the terminal rather than the notebook.

### Rubric Points
#### Does the project load the pretrained vgg model? 
The function load_vgg is implemented correctly.
#### Does the project learn the correct features from the images?
The function layers is implemented correctly.

#### Does the project optimize the neural network?
The function optimize is implemented correctly.

#### Does the project train the neural network?
The function train_nn is implemented correctly. The loss of the network should be printed while the network is training.

#### Does the project train the model correctly?
The network is trained using the train_nn (from line 140 to line 174) using keep probability 0.5 and learning rate 0.00001 with  6, 12, 24 and 48 epochs

#### Does the project use reasonable hyperparameters?

Learning rate = 0.00001
Epochs = 6, 12, 24 and 48

#### Does the project correctly label the road?
Yes

### Reference
Some of the project ideas has been taken from https://github.com/darienmt/CarND-Semantic-Segmentation-P2