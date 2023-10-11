# EROSION-AND-DILATION

## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Load the necessary packages requiured for the implemtation of erosion and dilation on an image


### Step2:

Create the text image for the implemtation of erosion and dilation using cv2.putText function.
### Step3:

Create the structuring image for the implemtation of erosion and dilation on the text image.
### Step4:
Apply the erosion and dilation to the text image using cv2.erode and cv2.dilate.

### Step5:

Display the images of the erosion and dilation applied using the plt.imshow.

### Step6:
End the program.
 
## Program:

#### Developed by: Jeevitha
#### Register Number: 212222230054
##### Program to implement Erosion and Dilation using Python and OpenCV.

# Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```

# Create the Text using cv2.putText
```
img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img1,'jeevitha E',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img1)
plt.show()
```


# Create the structuring element
```
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
```



# Erode the image
```
image_erode1=cv2.erode(img1,kernel)
plt.axis('off')
plt.imshow(image_erode1)
plt.show()

```

# Dilate the image
```
mage_dilate1=cv2.dilate(img1,kernel)
plt.axis('off')
plt.imshow(image_dilate1)
plt.show()
```





## Output:

### Display the input Image
![image](https://github.com/Jeevithaelumalai/EROSION-AND-DILATION/assets/118708245/bac39cf9-e51c-4d6d-bdf8-519e7048868e)


### Display the Eroded Image

![image](https://github.com/Jeevithaelumalai/EROSION-AND-DILATION/assets/118708245/af43083c-445a-4e39-9fee-16313fb7c208)


### Display the Dilated Image
![image](https://github.com/Jeevithaelumalai/EROSION-AND-DILATION/assets/118708245/65a47820-7b3f-447b-8d50-3c49df8464d5)


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
