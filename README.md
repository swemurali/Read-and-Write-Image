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
```
 Developed By: M.Suwetha
 Register Number: 212221230112
```
i) #To Read,display the image
```
import cv2
color= cv2.imread('swe.jpg',1)
cv2.imshow('suwetha212221230112',color)
cv2.waitKey(0)
```
ii) #To write the image
```
import cv2
color= cv2.imread('swe.jpg',-1)
cv2.imwrite('swe.jpg',color)
```
iii) #Find the shape of the Image
```
import cv2
color=cv2.imread('swe.jpg',1)
print(color.shape)
```
iv) #To access rows and columns

```
import cv2
import random
img= cv2.imread('swe.jpg',-1)
for i in range(300):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('suwetha212221230112',img)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```
import cv2
img= cv2.imread('swe.jpg',-1)
tag = img[200:450,200:450]
img[150:400,150:400] = tag
cv2.imshow('suwetha212221230112',img)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image

![output](./pic-01.png)


### ii)Write the image

![output](./pic-04.png)

### iii)Shape of the Image

![output](./pic-05.png)

### iv)Access rows and columns

![output](./pic-02.png)

### v)Cut and paste portion of image

 ![output](./pic-03.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


