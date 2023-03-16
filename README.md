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
### Developed By: VIDYA NEELA.M
### Register Number: 212221230120
i) #To Read,display the image
```
import cv2
color= cv2.imread('mm.png',1)
cv2.imshow('212221230102',color)
cv2.waitKey(0)
```

ii) #To write the image
```
import cv2
color= cv2.imread('mm.png',-1)
cv2.imwrite('mm.png',color)
```

iii) #Find the shape of the Image
```
import cv2
color=cv2.imread('mm.png',1)
print(color.shape)
```
iv) #To access rows and columns

```
import cv2
import random
img= cv2.imread('mm.png',-1)
for i in range(300):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221230102 SITHI HAJARA',img)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```
import cv2
color=cv2.imread('mm.png',-1)
tag=color[200:300,200:300]
color[100:200,100:200]=tag
cv2.imshow('212221230102 SITHI HAJARA',color)
cv2.waitKey(0)
cv2.destroyAllWindows()

```

## Output:

### i) Read and display the image

<br>

<br>

### ii)Write the image

<br>

<br>

### iii)Shape of the Image

<br

<br>

### iv)Access rows and columns
<br>

<br>

### v)Cut and paste portion of image
<br>

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


