# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV


## Algorithm:
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
 
## Program:
```
/*
Developed by   : S. Sanjna Priya
Register Number: 212220230043
*/
```
# Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
# Create the Text using cv2.putText
```
image=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(image,'Sanjna',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(image)
plt.show()
```
# Create the structuring element
```
kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(9,9))
```
# Erode the image
```
image_erode1=cv2.erode(image,kernel)
plt.axis('off')
plt.imshow(image_erode1)
plt.show()
```
# Dilate the image
```
image_dilate1=cv2.dilate(image,kernel)
plt.axis('off')
plt.imshow(image_dilate1)
plt.show()
```

## Output:

### Display the input Image
![10 1](https://user-images.githubusercontent.com/75234965/170942631-f7b8771c-ed62-4f78-8ff8-3edfb7a7f686.PNG)

### Display the Eroded Image
![10 2](https://user-images.githubusercontent.com/75234965/170942691-5726ad40-c8f8-49b8-a347-87517e5c6420.PNG)

### Display the Dilated Image
![image](https://user-images.githubusercontent.com/75234965/170942789-4f4af010-0103-4888-a2d8-b99b882fa3a1.png)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
