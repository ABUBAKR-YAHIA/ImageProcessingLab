
# Power Law (Gamma) Transformations
“Gamma Correction”, most of you might have heard this strange sounding thing. In this blog, we will see what it means and why does it matter to you?

The general form of Power law (Gamma) transformation function is

s = c*rγ

If images are not gamma-encoded, they allocate too many bits for the bright tones that humans cannot differentiate and too few bits for the dark tones. So, by gamma encoding, we remove this artifact.

Images which are not properly corrected can look either bleached out, or too dark.

Let’s verify by code that γ <1 produces images that are brighter while γ >1 results in images that are darker than intended

## Code:

import numpy as np

import cv2

#Load the image

img = cv2.imread('forest.png')

#Apply Gamma=2.2 on the normalised image and then multiply by scaling constant (For 8 bit, c=255)

gamma_two_point_two = np.array(255*(img/255)**2.2,dtype='uint8')

#Similarly, Apply Gamma=0.4 

gamma_point_four = np.array(255*(img/255)**0.4,dtype='uint8')

#Display the images in subplots

img3 = cv2.hconcat([gamma_two_point_two,gamma_point_four])

cv2.imshow('a2',img3)

cv2.waitKey(0)




