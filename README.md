# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:

Import the necessary packages

### Step2:

Create the Text using cv2.putText

### Step3:

Create the structuring element

### Step4:

Use Opening operation

### Step5:

Use Closing Operation

 
## Program:

``` Python
Developed by : DEEPIKA R
Reg no : 212224100009

import cv2
import numpy as np
import matplotlib.pyplot as plt
img = np.zeros((100, 550), dtype = 'uint8')
font = cv2.FONT_ITALIC
cv2.putText(img, 'Ayisha Rinsi K', (5,70), font, 2, (255), 5, cv2.LINE_AA)
n_img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
plt.imshow(n_img)
plt.axis("off")
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS, (11,11)
image_open = cv2.morphologyEx(n_img, cv2.MORPH_OPEN, kernel)
plt.imshow(image_open)
plt.axis("off")

image_close = cv2.morphologyEx(n_img, cv2.MORPH_CLOSE, kernel)
plt.imshow(image_close)
plt.axis("off")






```
## Output:

### Display the input Image

<img width="624" height="113" alt="image" src="https://github.com/user-attachments/assets/b7834c36-704c-434f-a25b-8637783f80cd" />

### Display the result of Opening

<img width="629" height="127" alt="image" src="https://github.com/user-attachments/assets/fcc1dab5-c70f-433f-ab14-ffec94bdf59b" />


### Display the result of Closing

<img width="637" height="133" alt="image" src="https://github.com/user-attachments/assets/76880d6e-7ec6-4d23-bef3-d89792339e0f" />

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
