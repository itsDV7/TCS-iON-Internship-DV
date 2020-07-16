# TCS-iON-Remote-Internship
TCS Remote Internship. 210 Hours. Project Work.
- **Name:** Divyansh Chaudhary
- **Institute:** Amity University Noida
- **Project Title:** Automate identification and recognition of handwritten text from an image.
## Getting Started
To run the project on your local machine, you will require the exact build of packages as some of the functions used in this project work only on these builds and are updated/removed in latest builds.
### Prerequsites
1. Install [Python 3.7.6.](https://www.python.org/downloads/release/python-376/)
2. Add Python 3.7.6 to PATH.
3. Install [PyCharm IDE Community Version.](https://www.jetbrains.com/pycharm/download/#section=windows)
4. Add launcher directory to PATH during installation.
5. Create a blank project with base interpreter. `Python37/python.exe`
### Packages
```
- Keras         2.3.1
- matplotlib    3.1.3
- numpy         1.18.1
- opencv-python 4.2.0.32
- sklearn       0.0
- tensorflow    2.0.0
```
### Instructions
1. Download [File1.py](https://github.com/itsDV7/TCS-iON-Remote-Internship/blob/master/File1.py), [File2.py](https://github.com/itsDV7/TCS-iON-Remote-Internship/blob/master/File2.py) and [TestData.zip](https://github.com/itsDV7/TCS-iON-Remote-Internship/blob/master/TestData.zip) available in the [repo.](https://github.com/itsDV7/TCS-iON-Remote-Internship/)
2. Add them to your project directory.
3. Execute [File1.py](https://github.com/itsDV7/TCS-iON-Remote-Internship/blob/master/File1.py)
4. Execute [File2.py](https://github.com/itsDV7/TCS-iON-Remote-Internship/blob/master/File2.py)
5. Use your webcam to test the digits.
## Results
After executing [File1.py](https://github.com/itsDV7/TCS-iON-Remote-Internship/blob/master/File1.py), the result of your model can be seen as follows:
```
Model: "sequential_1"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d_1 (Conv2D)            (None, 28, 28, 60)        1560      
_________________________________________________________________
conv2d_2 (Conv2D)            (None, 24, 24, 60)        90060     
_________________________________________________________________
max_pooling2d_1 (MaxPooling2 (None, 12, 12, 60)        0         
_________________________________________________________________
conv2d_3 (Conv2D)            (None, 10, 10, 30)        16230     
_________________________________________________________________
conv2d_4 (Conv2D)            (None, 8, 8, 30)          8130      
_________________________________________________________________
max_pooling2d_2 (MaxPooling2 (None, 4, 4, 30)          0         
_________________________________________________________________
dropout_1 (Dropout)          (None, 4, 4, 30)          0         
_________________________________________________________________
flatten_1 (Flatten)          (None, 480)               0         
_________________________________________________________________
dense_1 (Dense)              (None, 500)               240500    
_________________________________________________________________
dropout_2 (Dropout)          (None, 500)               0         
_________________________________________________________________
dense_2 (Dense)              (None, 10)                5010      
=================================================================
Total params: 361,490
Trainable params: 361,490
Non-trainable params: 0
```
The accuracy of the trained model can be checked from console:
```
Test Score =  0.003487161887470976
Test Accuracy =  0.999015748500824
```
Finally, [File2.py](https://github.com/itsDV7/TCS-iON-Remote-Internship/blob/master/File2.py) is executed to test the model with new examples.
