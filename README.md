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
### Developed By: Gunaseelan G
### Register Number: 212221230031
i) #To Read,display the image
```python
import cv2
color_image=cv2.imread("ducati.jpg",1)
cv2.imshow("2122212300",color_image)
cv2.waitKey(0)
  
```
ii) #To write the image
import cv2
color_image = cv2.imread('ducati.jpg',1)
h = cv2.imwrite('ducati.jpg',color_image)
cv2.imshow('super',color_image)
cv2.waitKey(0) 


iii) #Find the shape of the Image
import cv2
color_image = cv2.imread('ducati.jpg',1)
print(color_image.shape)


iv) #To access rows and columns

import random
import cv2
color_image = cv2.imread('ducati.jpg',1)
for i in range(150):
    for j in range(color_image.shape[1]):
        color_image[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('ducati.jpg',color_image)
cv2.waitKey(0)



v) #To cut and paste portion of image
import cv2
color_image = cv2.imread('ducati.jpg',1)
part = color_image[300:400,300:400]
color_image[50:150,50:150] = part
cv2.imshow("superbike",color_image)
cv2.waitKey(0)





## Output:

### i) Read and display the image
![output1](https://user-images.githubusercontent.com/93427255/225330883-8896a270-385b-4564-a673-971956be4c20.png)


### ii)Write the image

![output2](https://user-images.githubusercontent.com/93427255/225330954-bff42103-6c3f-4f31-a177-4962ef8831a9.png)


### iii)Shape of the Image

![output3](https://user-images.githubusercontent.com/93427255/225331025-d11e17e6-a87a-43f1-9885-fc64d781260d.png)


### iv)Access rows and columns
![output4](https://user-images.githubusercontent.com/93427255/225331059-3589cbad-8f53-404d-b76f-0dadd9ead1ab.png)


### v)Cut and paste portion of image
![output5](https://user-images.githubusercontent.com/93427255/225331092-6c05cca2-1ab2-49f2-a5ce-01a33d8499f7.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


