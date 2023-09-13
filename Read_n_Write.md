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
```
image=cv2.imread("pain.jpg",1)
cv2_imshow(image)  

```
ii) #To write the image
```
image = cv2.imread("pain.jpg",-1)
cv2.imwrite("pain.jpg",image)


```
iii) #Find the shape of the Image
```python3
print(image.shape)


```
iv) #To access rows and columns

```python3

for i in range(150):
    for j in range(image.shape[1]):
        image[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2_imshow(image)
cv2.waitKey(0)

```
v) #To cut and paste portion of image
```python3
image= cv2.imread('bike.jpg',-1)
new = image[200:450,200:450]
image[150:400,150:400] = new
cv2_imshow(image)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image

<br>

![](obito.jpg)

<br>

### ii)Write the image

<br>

![](Img_Write.png)

<br>

### iii)Shape of the Image

<br>

![](img_shape.png)

<br>

### iv)Access rows and columns
<br>

![](noise_obito.png)
<br>

### v)Cut and paste portion of image
<br>

![](sq_obito.png)

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


