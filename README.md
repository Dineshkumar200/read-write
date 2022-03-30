# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
```python
# Developed By:Dineshkumar V
# Register Number:212220230013
# To Read,display the image
import numpy as np
import cv2
img = cv2.imread('k.jpg',1)
cv2.imshow('image',img)
cv2.waitKey(0)


# To write the image

cv2.imwrite('dk.jpg',img)


# Find the shape of the Image

print(img.shape)




# To access rows and columns
import random
for i in range(100):
    for j in range(img.shape[1]):
        img[i][j]= [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('image',img)
cv2.waitKey(0)


# To cut and paste portion of image

bw2=cv2.imread("k.jpg",1)
tag=bw2[30:100,30:120]
bw2[50:120,100:190]=tag
cv2.imshow("cutting portion",bw2)
cv2.waitKey(0)
cv2.destroyAllWindows()










```
## Output:

### i) Read and display the image



![g1](https://user-images.githubusercontent.com/75235789/160869249-2d4b6302-30fa-4269-b473-1ffa14229774.jpg)


### ii)Write the image

![g2](https://user-images.githubusercontent.com/75235789/160869306-41aad4f1-a397-4c73-b16d-fbbddbd76a1c.jpg)


### iii)Shape of the Image

![g2](https://user-images.githubusercontent.com/75235789/160869370-080dd026-8c7f-45b0-ba21-201de427530a.jpg)


### iv)Access rows and columns
![g3](https://user-images.githubusercontent.com/75235789/160869346-ccb0e264-ebcd-44dc-8c81-687c767f9c54.jpg)


### v)Cut and paste portion of image
![g4](https://user-images.githubusercontent.com/75235789/160869404-4d3e493c-a007-4e76-ab3c-bbf432988228.jpg)


## Result:
Thus the images are read, displayed, and written successfully using the python program.




