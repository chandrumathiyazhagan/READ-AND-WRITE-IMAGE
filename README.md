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
### Developed By:
### Register Number: 
i) #To Read,display the image
```python
import cv2
image=cv2.imread("mk.jpeg",1)
cv2.imshow("212222230026_M.Chandru",image)
cv2.waitKey(0)
cv2.destroyAllwindows()  

```
ii) #To write the image
```python

import cv2
image=cv2.imread("mk.jpeg",1)
cv2.imwrite("mk.jpeg",image)
cv2.imshow("212222230026_M.Chandru",image)
cv2.waitKey(0)
cv2.destroyAllwindows()

```
iii) #Find the shape of the Image
```python3

import cv2
picture=cv2.imread("mk.jpeg",1)
print(picture.shape)

```
iv) #To access rows and columns

```python3

import random
import cv2
image=cv2.imread("mk.jpeg",1)
for i in range(100):
    for j in range(image.shape[1]):
        image[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("212222230026_M.Chandru",image)
cv2.waitKey(0)
cv2.destroyAllwindows()

```
v) #To cut and paste portion of image
```python3

import cv2
img = cv2.imread('mk1.jpeg', 1)
tag = img[20:80:, 20:80]
img[90:150, 90:150] = tag
cv2.imshow('212222230026_M.Chandru', img)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image
![Screenshot from 2023-08-23 13-34-24](https://github.com/chandrumathiyazhagan/READ-AND-WRITE-IMAGE/assets/119393023/84ec4ed1-abd0-4d06-8f6b-8f3978703d20)

<br>
<br>

### ii)Write the image
![Screenshot from 2023-08-23 14-28-40](https://github.com/chandrumathiyazhagan/READ-AND-WRITE-IMAGE/assets/119393023/ba8fb996-7ca3-4150-a55a-79b7ae6c28e5)

<br>
<br>

### iii)Shape of the Image
![Screenshot from 2023-08-23 13-36-02](https://github.com/chandrumathiyazhagan/READ-AND-WRITE-IMAGE/assets/119393023/b49e4408-2e7b-4ae6-9a8d-bb220d6891c9)

<br>
<br>

### iv)Access rows and columns
![Screenshot from 2023-08-23 14-30-05](https://github.com/chandrumathiyazhagan/READ-AND-WRITE-IMAGE/assets/119393023/82041321-1712-40fe-a6e4-be04a0b5ea43)

<br>
<br>


### v)Cut and paste portion of image
![212222230026_M Chandru_screenshot](https://github.com/chandrumathiyazhagan/READ-AND-WRITE-IMAGE/assets/119393023/e895e8a3-a1e6-4461-bb8f-f924ec19a759)
<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.
