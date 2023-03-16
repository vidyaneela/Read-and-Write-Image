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
cv2.imshow('212221230120',color)
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
cv2.imshow('212221230120 VIDYANEELA',img)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```
import cv2
color=cv2.imread('mm.png',-1)
tag=color[200:300,200:300]
color[100:200,100:200]=tag
cv2.imshow('212221230120 VIDYA NEELA',color)
cv2.waitKey(0)
cv2.destroyAllWindows()

```

## Output:

### i) Read and display the image

![image](https://user-images.githubusercontent.com/94169318/225517807-76244931-f928-41a6-a014-0ef99a9b41c9.png)


### ii)Write the image

![image](https://user-images.githubusercontent.com/94169318/225517833-bd264910-4111-49d0-931e-80119b782fbd.png)


### iii)Shape of the Image

![image](https://user-images.githubusercontent.com/94169318/225517676-6313d83c-5b8c-4a39-b73b-93b6002fec74.png)


### iv)Access rows and columns

![image](https://user-images.githubusercontent.com/94169318/225517706-23d3661c-fb8b-45e2-8a19-c19f88e32a79.png)


### v)Cut and paste portion of image

![image](https://user-images.githubusercontent.com/94169318/225517761-3c654d94-9cbe-41a6-8393-01e46b66b4b1.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


