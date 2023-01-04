- Convolutional neural networks are a specialized type of artificial neural networks that use a mathematical operation called convolution in place of general matrix multiplication in at least one of their layers. They are specifically designed to process pixel data and are used in image recognition and processing. CNNs are used for image classification and recognition because of its high accuracy.
![[Pasted image 20230104073929.png|center|700]]
![[Pasted image 20230104094637.png|center|700]]
```ad-note
The objective of the Convolution Operation is to **extract the high-level features** such as edges, from the input image. ConvNets need not be limited to only one Convolutional Layer. Conventionally, the first ConvLayer is responsible for capturing the Low-Level features such as edges, color, gradient orientation, etc. With added layers, the architecture adapts to the High-Level features as well, giving us a network that has a wholesome understanding of images in the dataset, similar to how we would.
```
```ad-note
In convolutional layers the weights are represented as the multiplicative factor of the filters.
For example, if we have the input 2D matrix in green
![[Pasted image 20230104094339.png]]
with the convolution filter
![[Pasted image 20230104094352.png]]
Each matrix element in the convolution filter is the weights that are being trained. These weights will impact the extracted convolved features as
![[s47gB.gif]]
```
```ad-note
Similar to the Convolutional Layer, the Pooling layer is responsible for reducing the spatial size of the Convolved Feature. This is to **decrease the computational power required to process the data** through dimensionality reduction. Furthermore, it is useful for **extracting dominant features** which are rotational and positional invariant, thus maintaining the process of effectively training the model.
```
```ad-note
In the classification part, the flattened output is fed to a feed-forward neural network and backpropagation is applied to every iteration of training. Over a series of epochs, the model is able to distinguish between dominating and certain low-level features in images and classify them using the **Softmax Classification** technique.
```