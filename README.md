# NeStEr
###
This is a project that sees the working of a CNN model that was utilised in large numbers by school students to design their own art work of loitering around with 2 different pictures and combining them to generate a single master piece. Used VGG Neural Network (read more about it below) , NST (read more about it below) and tensorflow to build it.
#
# VGG Neural Network
###
VGG16 is a convolutional neural network model proposed by K. Simonyan and A. Zisserman from the University of Oxford in the paper “Very Deep Convolutional Networks for Large-Scale Image Recognition”. The model achieves 92.7% top-5 test accuracy in ImageNet, which is a dataset of over 14 million images belonging to 1000 classes.


### VGG16 Architecture
The input to cov1 layer is of fixed size 224 x 224 RGB image. The image is passed through a stack of convolutional (conv.) layers, where the filters were used with a very small receptive field: 3×3 (which is the smallest size to capture the notion of left/right, up/down, center). In one of the configurations, it also utilizes 1×1 convolution filters, which can be seen as a linear transformation of the input channels (followed by non-linearity). The convolution stride is fixed to 1 pixel; the spatial padding of conv. layer input is such that the spatial resolution is preserved after convolution, i.e. the padding is 1-pixel for 3×3 conv. layers. Spatial pooling is carried out by five max-pooling layers, which follow some of the conv.  layers (not all the conv. layers are followed by max-pooling). Max-pooling is performed over a 2×2 pixel window, with stride 2.

Three Fully-Connected (FC) layers follow a stack of convolutional layers (which has a different depth in different architectures): the first two have 4096 channels each, the third performs 1000-way ILSVRC classification and thus contains 1000 channels (one for each class). The final layer is the soft-max layer. The configuration of the fully connected layers is the same in all networks. The illustration for the same can be seen below : 
###
###
###
<a href="https://neurohive.io/en/popular-networks/vgg16/"><img src="https://neurohive.io/wp-content/uploads/2018/11/vgg16-neural-network.jpg" title="VGG16 Architecture"></a>

#
# Neural Style Transfer technique (NST)
###
Neural style transfer is an optimization technique used to take two images—a content image and a style reference image (such as an artwork)—and blend them together so the output image looks like the content image, but “painted” in the style of the style reference image.

This is implemented by optimizing the output image to match the content statistics of the content image and the style statistics of the style reference image. These statistics are extracted from the images using a convolutional network.
The code sees the implementation of neural style transfer technique and is one of the best projects I have worked on!!
The code takes in 2 images as an input and returns a third image which is a blend (combination) of both the input images.
###
### So here's an example illustrating the same : 
###
<a href="https://www.tensorflow.org/tutorials/generative/style_transfer"><img src="https://www.tensorflow.org/tutorials/generative/style_transfer_files/output__UWQmeEaiKkP_0.png" title="VGG16 Architecture"></a>
### Contant Image + Style Image = Final image 

<a href="https://www.tensorflow.org/tutorials/generative/style_transfer"><img src="https://www.tensorflow.org/tutorials/generative/style_transfer_files/output_iYSLexgRKSh-_0.png" title="VGG16 Architecture"></a>
 
#

I hope you'll enjoy the output of your own pictures executed more than just the example here. So, why wait more? Just follow the code which is already been well explained with comments inside and enjoy!!!!

My motivation for working on this project was driven by the students of my school who face a little difficulty in coming up with "COOL" backgrounds for making posters for varoius events using photoshop!! 

Hope you'll like and appreciate the amazing technique!! :)
