# Convolutional-ResNet-Models

Implement the basic building ResNets (50 layers)

* Zero-padding pads the input with a pad of (3,3)
* The 2D Convolution has 64 filters of shape (7,7) and uses a stride of (2,2). Its name is "conv1".
BatchNorm is applied to the channels axis of the input.
MaxPooling uses a (3,3) window and a (2,2) stride.
* The convolutional block uses three set of filters of size [64,64,256], "f" is 3, "s" is 1 and the block is "a".
The 2 identity blocks use three set of filters of size [64,64,256], "f" is 3 and the blocks are "b" and "c".
* The convolutional block uses three set of filters of size [128,128,512], "f" is 3, "s" is 2 and the block is "a".
The 3 identity blocks use three set of filters of size [128,128,512], "f" is 3 and the blocks are "b", "c" and "d".
* The convolutional block uses three set of filters of size [256, 256, 1024], "f" is 3, "s" is 2 and the block is "a".
The 5 identity blocks use three set of filters of size [256, 256, 1024], "f" is 3 and the blocks are "b", "c", "d", "e" and "f".
* The convolutional block uses three set of filters of size [512, 512, 2048], "f" is 3, "s" is 2 and the block is "a".
The 2 identity blocks use three set of filters of size [512, 512, 2048], "f" is 3 and the blocks are "b" and "c".
* The 2D Average Pooling uses a window of shape (2,2) and its name is "avg_pool".
* The flatten doesn't have any hyperparameters or name.
*The Fully Connected (Dense) layer reduces its input to the number of classes using a softmax activation. Its name should be 'fc' + str(classes).
