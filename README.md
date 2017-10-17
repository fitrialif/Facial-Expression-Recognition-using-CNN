# Facial-Expression-Recognition-using-CNN

Project about mood recognition using convolutional neural network for my college project

## Dependencies

- [NumPy](http://docs.scipy.org/doc/numpy-1.10.1/user/install.html)
- [Tensorflow](https://www.tensorflow.org/versions/r0.8/get_started/os_setup.html)
- [TFLearn](https://github.com/tflearn/tflearn#installation)
- [OpenCV](https://opencv-python-tutroals.readthedocs.io/en/latest/)

## Dataset

-FER2013 dataset [Kraggle](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data).

## Usage
* Divide the FER2013 dataset into training and testing set.
  * I divided the dataset manually by copy pasting the csv file content in two different files.
  * Give the two file name as test.csv and train.csv respectively.
* Convert the .csv files to npy object by running csv-npy.py
  * Note: you need to do this step twice, once for test.csv and then for train.csv
  * (Dont forget change the file names in the csv-npy.py program when running the second time for test.csv)
```bash
$ python csv-npy.py
```
  
* Train the CNN by running training.py 
```bash
$ python training.py
```
  ##### Note:
    * Once the training of cnn is complete the program will create some files in the temp folder.
    * All the steps above are only required to be performed once.
    * Once the temp files are created then you can run the code below.
* Run the Recdelay.py
```bash
$ python recdelay.py
```

