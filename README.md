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
### Developed By:Roshini RK
### Register Number: 212222230123
i) #To Read,display the image
```python3
 import cv2
img = cv2.imread('d.jpg', 1)
cv2.imshow('212222230123_Roshini', img)
cv2.waitKey(0) 

```
ii) #To write the image
```python3
import cv2
img = cv2.imread('d.jpg', 1)
new_img = cv2.imwrite('d_c.jpg', img)
cv2.imshow('212222230123_Roshini', img)
cv2.waitKey(0)


```
iii) #Find the shape of the Image
```python3
import cv2
img = cv2.imread('d.jpg', 1)
print(img.shape)


```
iv) #To access rows and columns

```python3
import cv2
import random
img = cv2.imread('d.jpg', 1)
for i in range(100):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0, 255), random.randint(0, 255), random.randint(0, 255)]
cv2.imshow('part image', img)
cv2.waitKey(0)
cv2.destroyAllWindows()


```
v) #To cut and paste portion of image
```python3
import cv2
img = cv2.imread('d.jpg', 1)
tag = img[300:400, 300:400]
img[50:150, 50:150] = tag
cv2.imshow('212222230123_Roshini', img)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image

<br>

![image](https://github.com/roshiniRK/READ-AND-WRITE-IMAGE/assets/118956165/a0f0efb9-9975-4a82-8ed2-f877344b3750)


<br>

### ii)Write the image

<br>

![image](https://github.com/roshiniRK/READ-AND-WRITE-IMAGE/assets/118956165/d12dbf9a-4b29-4a76-ab4d-529c57b188e0)



<br>

### iii)Shape of the Image

<br>

![image](https://github.com/roshiniRK/READ-AND-WRITE-IMAGE/assets/118956165/0e893a78-530e-4497-8f05-7ba3ca5bc6d8)

<br>

### iv)Access rows and columns
<br>

![image](https://github.com/roshiniRK/READ-AND-WRITE-IMAGE/assets/118956165/b0acf238-943e-4183-92f0-b54876e298ef)


### v)Cut and paste portion of image
<br>

![image](https://github.com/roshiniRK/READ-AND-WRITE-IMAGE/assets/118956165/dd44b6bc-a972-49d9-b62b-6400a90d4f42)

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.
