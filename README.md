# IMPLEMENTATION OF EROSION AND DILATION
## AIM:
To implement Erosion and Dilation using Python and OpenCV.
## SOFTWARE REQUIRED:
1. Anaconda - Python 3.7
2. OpenCV
## ALGORITHM:
### Step 1:
Import the necessary packages.
### Step 2:
Create the Text using cv2.putText
### Step 3:
Create the structuring element.
### Step 4:
Erode the image.
### Step 5:
Dilate the image.

## PROGRAM:
```
/*
Developed by   : U Bhavya
Register Number: 212220230055
*/
```
``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img1,'U Bhavya',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img1)
plt.show()

# Create the structuring element
kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(9,9))

# Erode the image
image_erode1=cv2.erode(img1,kernel)
plt.axis('off')
plt.imshow(image_erode1)
plt.show()

# Dilate the image
image_dilate1=cv2.dilate(img1,kernel)
plt.axis('off')
plt.imshow(image_dilate1)
plt.show()
```
## OUTPUT:

### Display the input Image
![image](https://user-images.githubusercontent.com/75235293/169954532-6316ce97-b3a4-48e7-9de7-fd931ac17e71.png)


### Display the Eroded Image
![image](https://user-images.githubusercontent.com/75235293/169954604-fdea402d-e867-4829-a652-05660ab2ad18.png)


### Display the Dilated Image
![image](https://user-images.githubusercontent.com/75235293/169954697-72ed3ef0-6ea4-4805-bbef-5ea6dbca64d1.png)


## RESULT:
Thus the generated text image is eroded and dilated using python and OpenCV.
