## Negative transformation of an image using Python and OpenCV
Image is also known as a set of pixels. When we store an image in computers or digitally, it’s corresponding pixel values are stored. So, when we read an image to a variable using OpenCV in Python, the variable stores the pixel values of the image. When we try to negatively transform an image, the brightest areas are transformed into the darkest and the darkest areas are transformed into the brightest.

As we know, a color image stores 3 different channels. They are red, green and blue. That’s why color images are also known as RGB images. So, if we need a negative transformation of an image then we need to invert these 3 channels.

## Steps for negative transformation

1. Read an image
2. Get height and width of the image
3. Each pixel contains 3 channels. So, take a pixel value and collect 3 channels in 3 different variables.
4. Negate 3 pixels values from 255 and store them again in pixel used before.
5. Do it for all pixel values present in image.

## Outputs:
#### Orignal Image:
![output1](https://user-images.githubusercontent.com/72355871/105163495-d77a2f00-5ac8-11eb-8050-d72c78b30009.JPG)
#### Negative Image:
![output2](https://user-images.githubusercontent.com/72355871/105163494-d5b06b80-5ac8-11eb-8e40-984ae7c3a10b.JPG)
