# face_mask_detection_simple
A simple hack to detect face mask without training any custom machine learning algorithms!!

## **Summary:**

This project uses just openCV and numpy to detect face masks. I thought of training a CNN for face mask detection with 2 classes in the dataset(images with people wearing mask and the other not wearing). But we have classic haar-cascades for face, eyes and mouth detection.This can be an exampple for transfer learning:)    

So, I have used haar-cascades to:
--First, detect face in the frame
--Detect Eyes in that face
--Detect mouth in the frame
--Now, a simple if condition:
    if face and eyes are present but mouth isn't, the person is wearing a mask
    else if face, eyes and mouth are detected, the person is wearing a mask
    
Haar cascades are not very accurate, but it can do it's job. I have tuned the parameters such that it works fine when the face that's being detected is sitting in front of the webcame(like the screenshot below). 
## **Screenshots:**
Homepage:

![alt text]()

