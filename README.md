## Image Segmentation

#### Dataset
The dataset used is plant village dataset : 
https://www.kaggle.com/vipoooool/new-plant-diseases-dataset

#### Properties of images

Type of File : JPG File.

Dimensions : 256 * 256.

Width : 256 Pixels.

Height : 256 Pixels.

Horizontal Resolution : 96 dpi.

Vertical Resolution : 96 dpi.

Bit Depth : 24.

#### Steps Involved 
1. Load original image.

2. Conversion of image from RGB to BGR. Since Open CV (python library for Image Processing), accepts images in BGR coloring format so it needs to be converted to the BGR format.

3. Conversion of image from BGR to HSV. The simple answer is that unlike RGB, HSV separates luma, or the image intensity, from chroma or the color information. This is very useful in many applications. For example, if you want to do histogram equalization of a color image, you probably want to do that only on the intensity component, and leave the color components alone. Otherwise you will get very strange colors. In computer vision you often want to separate color components from intensity for various reasons, such as robustness to lighting changes, or removing shadows. Note, however, that HSV is one of many color spaces that separate color from intensity (See YCbCr, Lab, etc.). HSV is often used simply because the code for converting between RGB and HSV is widely available and can also be easily implemented.

4. Image Segmentation for extraction of Colors. In order to separate the picture of leaf from the background segmentation has to performed, The color of the leaf is extracted from the image.
