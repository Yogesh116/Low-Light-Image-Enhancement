# Low-Light-Image-Enhancement-Project 
Due to low lighting circumstances, images recorded in outdoor scenes can be severely affected. Low dynamic range and excessive noise levels in these photos can influence the overall effectiveness of computer vision systems. Use low-light image enhancement to improve the visibility of an image to make computer vision algorithms more robust in low-light circumstances.

In this notebook, we are using many Deep neural network layers to enhance low-light images, extracting a parameter map the same size as the image.

# Dataset
We worked on LOL Dataset.And you can download the dataset click on this link - https://drive.google.com/file/d/157bjO1_cFuSd0HWDUuAmcHRJDVyWpOxB/view.

# Dependecies
numpy,<br>
opencv<br>
imageio<br>
glob <br>
matplotlib <br>
scipy <br>
tensorflow.keras.models.

# Deep Neural Network Model
We employ a plain CNN of seven convolutional
layers with symmetrical concatenation. Each layer
consists of 32 convolutional kernels of size 3x3 and stride<br>
1. Followed by the ReLU activation function. <br> 
2. The last convolutional layer is followed by the sigmoid activation function which produce parameter map of pixel range [0:1].<br>
3. We used the Adam optimizer and Mean Squarred Error loss function.


# We converted this steps of iterations into recursive function.
img: the low light image (**I**, **E**old) <br/>
index: no of iterations <br/>
flag: default = 1.

# Iteration Wise Examples
>LOL Dataset Image.

 ![README_17_1](https://user-images.githubusercontent.com/66743388/121814561-5269ff00-cc8f-11eb-8c89-6c46f6b33682.png)

# Some Example
>After 12 iteration
 ![12](https://user-images.githubusercontent.com/66743388/121814224-804e4400-cc8d-11eb-9604-fc70e2917b36.png)

>After 8 iteration
 ![8](https://user-images.githubusercontent.com/66743388/121814475-edaea480-cc8e-11eb-9690-9c813c63b9f4.png)

>After 7 iteration.
 
 ![7](https://user-images.githubusercontent.com/66743388/121814616-a2e15c80-cc8f-11eb-8e3a-b657f98dd3b3.png)




