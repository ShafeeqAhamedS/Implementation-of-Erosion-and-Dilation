# <p align="center">Implementation of Erosion and Dilation</p>

## Aim
To implement Erosion and Dilation using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm:
### Step1:
Import the necessary packages.
### Step2:
Create the Text using cv2.putText.
### Step3:
Create the structuring element.
### Step4:
Erode and Dilate the image.
### Step5:
End Program.

</br>
</br>
</br>
</br>
</br>
</br>

## Program:
Developed By   : **Shafeeq Ahamed. S**
</br>

Register Number: **212221230092**

### Import the necessary packages
```py
import cv2
import numpy as np
from matplotlib import pyplot as plt
```
### Create the text using cv2.putText
```py
img1 = np.zeros((100,550), dtype = 'uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'Shafeeq Ahamed',(5,70), font, 2,(255),5,cv2.LINE_AA)
plt.imshow(img1,'gray')
```
### Create the structuring element
```py
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
cv2.erode(img1, kernel)
```
### Erode the image
```py
image_erode1 = cv2.erode(img1,kernel)
plt.imshow(image_erode1, 'gray')
```
### Dilate the image
```py
image_dilate1 = cv2.dilate(img1, kernel)
plt.imshow(image_dilate1, 'gray')
```

</br>
</br>
</br>
</br>
</br>
</br>

## Output:
### Display the input Image
![image](https://github.com/ShafeeqAhamedS/Implementation-of-Erosion-and-Dilation/assets/93427237/1cd2603b-ea43-407e-8df4-fa42095aa115)
### Display the Eroded Image
![image](https://github.com/ShafeeqAhamedS/Implementation-of-Erosion-and-Dilation/assets/93427237/5af7e26d-f956-4667-bf99-4c4987b561ac)
### Display the Dilated Image
![image](https://github.com/ShafeeqAhamedS/Implementation-of-Erosion-and-Dilation/assets/93427237/b67027d5-3b29-463d-bbd0-539ae5f39356)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
