# Facial Expressions Detection using YOLOv5

Facial expressions recognition using YOLOv5 and custom dataset with Roboflow - based on CKplus famous dataset.

## Custom Dataset

In this project, I took the famous CKplus facial expressions dataset from Kaggle.
This dataset contains 981 images with a size of 48x48.<br>
It contains 7 basic facial expressions:
- anger
- contempt
- disgust
- fear
- happy
- sad
- surprise<br>

The annotation was executed with Roboflow, so in the end of the process, I had a custom yaml file in YOLOv5 format, so the model will know how to differ between the different emotions.<br>
With Roboflow, I managed to implement various augmentations upon the dataset, so that it is vary diversified.
Therefore, the model will be more resilient and capable of dealing with frames with high brightness, blur, different rotations and angles, concealments and noise.  

A summarization of the custom dataset generation:<br>
![image](https://user-images.githubusercontent.com/121958931/220621185-742bbd55-6ca4-4460-9d4d-206a5c5b4f5b.png)

## Setup

1. Clone YOLOv5 base code and install requirements:<br>
![image](https://user-images.githubusercontent.com/121958931/220623068-2c03e551-7975-4143-8749-3d4c61bcb478.png)

2. Import the desired packages and connect to ROBOFLOW:<br>
![image](https://user-images.githubusercontent.com/121958931/220625748-0c2946ce-ff41-4352-b735-33004ec3aac4.png)

3. Train our custom YOLOv5 model:<br>
![image](https://user-images.githubusercontent.com/121958931/220623580-77dcff85-326e-4963-a5ce-adad311ab7ec.png)

![image](https://user-images.githubusercontent.com/121958931/220623656-958d8ab9-9b40-4c3d-9975-987ccb13de92.png)

The training process:<br>
![image](https://user-images.githubusercontent.com/121958931/220623825-8d608dbb-1d37-4906-b90a-d519f1afc40b.png)

4. Run model with trained weights:<br>
![image](https://user-images.githubusercontent.com/121958931/220623926-7d550aad-fa4f-4e89-ac60-d572130f20f0.png)

## Results 

![image](https://user-images.githubusercontent.com/121958931/220618324-5f5c85d8-5ec1-4fd5-b941-ea2ff3e8e94d.png)
![image](https://user-images.githubusercontent.com/121958931/220618338-cffbf9f7-c420-4d00-9275-b457f768615b.png)
![image](https://user-images.githubusercontent.com/121958931/220618359-9569ed01-4bd0-4e6b-b0f2-d01355a1e339.png)
![image](https://user-images.githubusercontent.com/121958931/220618377-00fcd2c4-b9e9-4c26-ab55-dc9092aca2ce.png)
![image](https://user-images.githubusercontent.com/121958931/220618387-8641d0dd-9b1c-463e-94d1-7715b745784a.png)
![image](https://user-images.githubusercontent.com/121958931/220618400-a8958229-d19d-44cf-a066-ba1a7a1449d7.png)
![image](https://user-images.githubusercontent.com/121958931/220618422-117a0490-9d2b-45b6-afe5-d60d865dc59e.png)

## Summary and Conclusions

With the creation of a custom dataset, and YOLOv5 algorithm of object detection - the detection of thease seven emotions, was a success.
In future versions, I will expand the amount of emotions to be detect and will try different additional augmentations techniques.
