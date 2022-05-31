# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
<br>


### Step2:
<br>

### Step3:
<br>

### Step4:
<br>

### Step5:
<br>

 
## Program:

``` Python

#Developed by : Revathi D
#Register number : 212221240045
# Import the necessary packages
import numpy as np
import cv2
import matplotlib.pyplot as plt
# Load the Image
img1=np.zeros((100,600),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL
# Create the Text using cv2.putText
cv2.putText(img1,' REVATHI ',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.imshow(img1,cmap='gray')
plt.title('Input Text'), plt.xticks([]), plt.yticks([])
plt.show()
# Create the structuring element
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
# Erode the image
img_erode=cv2.erode(img1,kernel1)
plt.imshow(img_erode,cmap='gray')
plt.title('Eroded Text'), plt.xticks([]), plt.yticks([])
plt.show()
# Dilate the image
img_dilate=cv2.dilate(img1,kernel1)
plt.imshow(img_dilate,cmap='gray')
plt.title('Dilated Text'), plt.xticks([]), plt.yticks([])
plt.show()




```
## Output:

### Display the input Image
![RE1](https://user-images.githubusercontent.com/96000574/171106730-fac32430-eaff-417b-935b-479078afc3ef.png)

### Display the Eroded Image
![RE2](https://user-images.githubusercontent.com/96000574/171106747-9c95770f-7999-428e-97bc-ecff8e62ef2e.png)


### Display the Dilated Image
![RE3](https://user-images.githubusercontent.com/96000574/171106781-d98ae80d-0de6-4240-82bd-50500688a4a9.png)


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
