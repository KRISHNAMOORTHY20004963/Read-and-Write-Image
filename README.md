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
### Developed By:KRISHNA MOORTHY.S
### Register Number:212220230025
i) #To Read,display the image
```
import cv2
img = cv2.imread('kimo1.jpg',1)
cv2.imshow('image',img)
cv2.waitKey(0)

```
ii) #To write the image
```

cv2.imwrite('kimo.jpg',img)

```
iii) #Find the shape of the Image
```python3

print(img.shape)

```
iv) #To access rows and columns

```python3

import random
for i in range(100):
    for j in range(img.shape[1]):
        img[i][j]= [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('image',img)
cv2.waitKey(0)

```
v) #To cut and paste portion of image
```python3

bw2=cv2.imread("kimo1.jpg",1)
tag=bw2[30:100,30:120]
bw2[50:120,100:190]=tag
cv2.imshow("cutting portion",bw2)
cv2.waitKey(0)
cv2.destroyAllWindows()

```

## Output:

### i) Read and display the image
![krishna1](https://user-images.githubusercontent.com/75241177/162247125-954ded84-751b-458f-9aef-4e682d8393b8.jpg)


### ii)Write the image

![krishna1](https://user-images.githubusercontent.com/75241177/162247157-97d9a389-50a8-496f-9a6f-709a737a3863.jpg)

### iii)Shape of the Image
![krishna1](https://user-images.githubusercontent.com/75241177/162247187-817b6988-cc60-4d5c-a3b7-143903a8e6ff.jpg)


### iv)Access rows and columns
![krishna2](https://user-images.githubusercontent.com/75241177/162247256-f2751281-fee8-490a-824c-155eb5d6af68.jpg)


### v)Cut and paste portion of image
![krishna3](https://user-images.githubusercontent.com/75241177/162247314-b533556b-83c0-4e3f-bd62-eecb947beb39.jpg)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


