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
### Developed By:Balireddy Mahalakshmi
### Register Number:212221240008
i) #To Read,display the image
```
  import cv2
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
cv2.imshow('212221240008-Read&Display',colorImage)
cv2.waitKey(0)

```
ii) #To write the image
```
import cv2
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
cv2.imwrite('/Users/eswar1607/Desktop/written.jpg',colorImage)
writtenImage = cv2.imread('/Users/eswar1607/Desktop/written.jpg',1)
cv2.imshow('212221240008-WrittenImage',writtenImage)
cv2.waitKey(0)

```
iii) #Find the shape of the Image
```python3
import cv2
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
print(colorImage.shape)

```
iv) #To access rows and columns
```python3
import cv2
import random
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
for i in range(100):
    for j in range(colorImage.shape[1]):
        colorImage[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221240008-AccessingRowsAndColumns',colorImage)
cv2.waitKey(0)

```
v) #To cut and paste portion of image
```python3
import cv2
color_img = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
tag = color_img[50:250,100:300]
color_img[100:300,50:250] = tag
cv2.imshow('212221240008-CutAndPaste',color_img)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image

<br>
<img width="535" alt="Screenshot 2022-03-31 at 10 32 55 PM" src="https://user-images.githubusercontent.com/93427286/161114786-b1eae874-6482-4fc3-a586-4b1f04b84d3b.png">
<br>

### ii)Write the image

<br>
<img width="535" alt="Screenshot 2022-03-31 at 10 37 28 PM" src="https://user-images.githubusercontent.com/93427286/161115459-28af641f-fb41-4b8d-a098-2bb1651d366d.png">

### iii)Shape of the Image

<br>
<img width="835" alt="Screenshot 2022-03-31 at 10 38 05 PM" src="https://user-images.githubusercontent.com/93427286/161115493-d29545e4-557d-4782-8a65-7a4ca477fa97.png">
<br>

### iv)Access rows and columns
<br>
<img width="535" alt="Screenshot 2022-03-31 at 10 38 53 PM" src="https://user-images.githubusercontent.com/93427286/161115568-c92f0f6e-cc25-4588-8ddc-4eb195b4c16d.png">
<br>

### v)Cut and paste portion of image
<br>
<img width="535" alt="Screenshot 2022-03-31 at 10 41 43 PM" src="https://user-images.githubusercontent.com/93427286/161115146-d73c3487-2367-4416-a06c-a8200dae3363.png">
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.
