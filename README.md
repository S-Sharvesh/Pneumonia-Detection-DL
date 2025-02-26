# Pneumonia Detection using Deep Learning

## Problem Statement

**Build a binary classifier to detect pneumonia using chest x-rays.**

### Pneumonia
> Pneumonia is an infection that inflames the air sacs in one or both lungs. The air sacs may fill with fluid or pus (purulent material), causing cough with phlegm or pus, fever, chills, and difficulty breathing. A variety of organisms, including bacteria, viruses and fungi, can cause pneumonia.  Chest X-ray, blood tests, and culture of the sputum may help confirm the diagnosis. The disease may be classified by where it was acquired, such as community- or hospital-acquired or healthcare-associated pneumonia.

## Dataset description

> The dataset is organized into 3 folders (train, test, val) and contains subfolders for each image category (Pneumonia/Normal). There are 5,863 X-Ray images (JPEG) and 2 categories (Pneumonia/Normal).
Chest X-ray images (anterior-posterior) were selected from retrospective cohorts of pediatric patients of one to five years old from Guangzhou Women and Children’s Medical Center, Guangzhou. All chest X-ray imaging was performed as part of patients’ routine clinical care. For the analysis of chest x-ray images, all chest radiographs were initially screened for quality control by removing all low quality or unreadable scans. The diagnoses for the images were then graded by two expert physicians before being cleared for training the AI system. In order to account for any grading errors, the evaluation set was also checked by a third expert.

### Dataset : https://www.kaggle.com/code/mohamedzayton/chest-xray/input

<img width="702" alt="image" src="https://github.com/user-attachments/assets/3318fd7f-9392-48f9-9e96-510fe9a380a8" />


## Model used :
**Here is a small comparison of all the models tested in the project:**

<img width="698" alt="image" src="https://github.com/user-attachments/assets/70f11c1f-58a3-499d-8afd-0ab989a06a74" />


- ### Convolutional Neural Network

![image](https://github.com/user-attachments/assets/cd15496a-92af-40d3-aba6-224326ba800e)


```
624/624 [==============================] - 11s 18ms/step
Loss of the model is -  0.30433156475042683
624/624 [==============================] - 10s 15ms/step
Accuracy of the model is -  91.98718070983887 %
```
<img width="707" alt="image" src="https://github.com/user-attachments/assets/18960510-da27-4a96-b0cb-304205caf7f6" />


- ### Convolutional Neural Network(Different approach) :

<img width="703" alt="image" src="https://github.com/user-attachments/assets/0d4a5920-ca5b-4055-b64d-dd22f3c355c9" />


```
624/624 [==============================] - 30s 49ms/step
Test Accuracy: 68.91%
652/652 [==============================] - 338s 518ms/step
Train Accuracy: 66.33%
```

- ### DenseNet :

<img width="701" alt="image" src="https://github.com/user-attachments/assets/d3e72c1e-f25d-4a13-8bce-49be5050cbad" />


<img width="701" alt="image" src="https://github.com/user-attachments/assets/f67b1232-8bd4-4172-8027-e477d5579daa" />



```
624/624 [==============================] - 132s 211ms/step
Test Accuracy: 87.18%
652/652 [==============================] - 622s 954ms/step
Train Accuracy: 86.22%
```
- ### VGG16 :

![image](https://github.com/user-attachments/assets/c2d2bfbf-4729-454c-be26-cc2f783c2d9f)

<img width="702" alt="image" src="https://github.com/user-attachments/assets/a7258d90-c804-4b32-b2fb-7825a9d3c9a5" />


```
624/624 [==============================] - 226s 363ms/step
Test Accuracy: 66.19%
652/652 [==============================] - 1608s 2s/step
Train Accuracy: 82.63%
```

- ### ResNet :

<img width="702" alt="image" src="https://github.com/user-attachments/assets/551f5e45-33d5-4ccb-b7a7-74c1696d483c" />

```
624/624 [==============================] - 101s 162ms/step
Test Accuracy: 73.40%
652/652 [==============================] - 651s 999ms/step
Train Accuracy: 88.92%
```

- ### InceptionNet :
<img width="702" alt="image" src="https://github.com/user-attachments/assets/3a374604-10a9-41d8-a344-638ca8805f9e" />

```
624/624 [==============================] - 41s 66ms/step
Test Accuracy: 76.76%
652/652 [==============================] - 295s 453ms/step
Train Accuracy: 91.26%
```
