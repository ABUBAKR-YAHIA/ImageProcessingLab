## Negative transformation of an image using Python and OpenCV
Image is also known as a set of pixels. When we store an image in computers or digitally, it’s corresponding pixel values are stored. So, when we read an image to a variable using OpenCV in Python, the variable stores the pixel values of the image. When we try to negatively transform an image, the brightest areas are transformed into the darkest and the darkest areas are transformed into the brightest.

As we know, a color image stores 3 different channels. They are red, green and blue. That’s why color images are also known as RGB images. So, if we need a negative transformation of an image then we need to invert these 3 channels.

#### Steps for negative transformation

[x] Read an image
[x] Get height and width of the image
[x] Each pixel contains 3 channels. So, take a pixel value and collect 3 channels in 3 different variables.
[x] Negate 3 pixels values from 255 and store them again in pixel used before.
[x] Do it for all pixel values present in image.
