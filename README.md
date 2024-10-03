# EDGE-DETECTION
## Aim:
To perform edge detection using Sobel, Laplacian, and Canny edge detectors.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import all the necessary modules for the program.

### Step2:
Load a image using imread() from cv2 module.

### Step3:
Convert the image to grayscale

### Step4:
Using Sobel operator from cv2,detect the edges of the image.

### Step5:

Using Laplacian operator from cv2,detect the edges of the image and Using Canny operator from cv2,detect the edges of the image.
## program:
Developed by:Balaji J
Register number:212221243001

## Convert image to grayscale and remove noise:
```
import cv2
import matplotlib.pyplot as plt
img=cv2.imread("parrot.jpeg",0)
gray=cv2.cvtColor(img,cv2.COLOR_GRAY2RGB)
gray = cv2.GaussianBlur(gray,(3,3),0)
```
## SOBEL EDGE DETECTOR
SOBEL X AXIS :
```
sobelx = cv2.Sobel(gray,cv2.CV_64F,1,0,ksize=5)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobelx)
plt.title("Sobel X axis")
plt.axis("off")
plt.show()
```
## SOBEL Y AXIS :
```
sobely = cv2.Sobel(gray,cv2.CV_64F,0,1,ksize=5)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobely)
plt.title("Sobel Y axis")
plt.axis("off")
plt.show()
```
## SOBEL XY AXIS :
```
sobelxy = cv2.Sobel(gray,cv2.CV_64F,1,1,ksize=5)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobelxy)
plt.title("Sobel XY axis")
plt.axis("off")
plt.show()
```
## LAPLACIAN EDGE DETECTOR:
```
lap=cv2.Laplacian(gray,cv2.CV_64F)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(lap)
plt.title("Laplacian Edge Detector")
plt.axis("off")
plt.show()
```

## CANNY EDGE DETECTOR:


```
canny=cv2.Canny(gray,120,150)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(canny)
plt.title("Canny Edge Detector")
plt.axis("off")
plt.show()
```


## Output:


### SOBEL EDGE DETECTOR
### SOBEL X AXIS:

![318662306-c4252422-c65a-425c-8ab6-8931e705b56a](https://github.com/user-attachments/assets/780aa109-5f23-4888-a5c0-01ace81d297c)


## SOBEL Y AXIS :


![318662447-c0c3b1a4-92dc-48e6-a6a6-62c6752ff7d3](https://github.com/user-attachments/assets/d9cc9dc4-0700-4e10-b21c-a59626d593af)


## SOBEL XY AXIS :


![318662648-e0a00353-1244-4ab6-b683-b6d98b175f4d](https://github.com/user-attachments/assets/dbf50b9e-35c1-4aac-9efa-c06a9f2556ec)

### LAPLACIAN EDGE DETECTOR

![318662776-7f15d807-2531-4116-8c46-c5971e4c5e29](https://github.com/user-attachments/assets/539bb311-9f5d-4ff8-b9da-62e3c26e67fa)


### CANNY EDGE DETECTOR

![318662893-31c32f1e-7e6d-40d5-bd58-efd09b665e0f](https://github.com/user-attachments/assets/e168594d-e834-461e-b304-1fa6956e0990)

## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.
