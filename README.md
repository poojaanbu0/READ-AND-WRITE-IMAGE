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
### Developed By: POOJA A
### Register Number: 212222240072
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
![WhatsApp Image 2023-11-14 at 02 27 01_df69aa54](https://github.com/poojaanbu0/READ-AND-WRITE-IMAGE/assets/119390329/ee88a2b2-5106-49d9-bd7c-4fc7976f439c)

### ii)Write the image
![WhatsApp Image 2023-11-14 at 02 29 25_35f84607](https://github.com/poojaanbu0/READ-AND-WRITE-IMAGE/assets/119390329/0a952da2-78ee-44ca-bdaf-2662df7bf107)


### iii)Shape of the Image
![WhatsApp Image 2023-11-14 at 02 29 41_e6771d2e](https://github.com/poojaanbu0/READ-AND-WRITE-IMAGE/assets/119390329/977fbd2d-30b8-4545-9d5b-58b431e4fe6b)

### iv)Access rows and columns
![WhatsApp Image 2023-11-14 at 02 30 06_c5970ada](https://github.com/poojaanbu0/READ-AND-WRITE-IMAGE/assets/119390329/f6b03fb8-3d8d-47f4-8d86-a1812a0462cb)


### v)Cut and paste portion of image
![WhatsApp Image 2023-11-14 at 02 30 34_54b32ff8](https://github.com/poojaanbu0/READ-AND-WRITE-IMAGE/assets/119390329/44fe307e-67c4-417d-a008-1fc8b8c41138)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


