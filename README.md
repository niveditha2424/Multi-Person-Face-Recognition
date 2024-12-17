# Multi-person Face Recognition From Blurred Images

## Introduction

This project focuses on developing a robust system for multi-person face recognition from blurred images. It involves several phases, including deblurring, face detection, and face recognition, each utilizing different algorithms and techniques.

## Deblurring Phase

In this phase, various deblurring methods were evaluated and compared based on parameters such as Mean Squared Error (MSE) and Peak Signal-to-Noise Ratio (PSNR). The methods tested include:

- Lucy Richardson Method
- Least Squares Method
- Wiener Method
- Blind Deconvolution Method

The results showed that the Lucy Richardson method provided the sharpest images, while the Wiener method offered better time complexity. A tradeoff between MSE and time complexity was observed.

## Face Detection

Two face detection models were compared in this phase: Haar-feature based cascade classifier and Multi-task Cascaded Convolutional Neural Network (MTCNN). The evaluation criteria included detection rate and computational time.

MTCNN outperformed Haar classifier in detection rate, especially in challenging scenarios like low-light conditions and partial faces. Although Haar classifier was faster, MTCNN was chosen for its higher accuracy.

## Face Recognition

Different face recognition models were trained and tested:

- AlexNet
- Modified AlexNet
- Custom Convolutional Neural Network (CNN)

These models were evaluated based on accuracy, computational time, and misclassification rate. While AlexNet achieved good accuracy, it struggled with crowded or overlapping faces. The Modified AlexNet improved accuracy but was slower. The Custom CNN processed faster but with more misclassifications.

## Results and Discussion

The results from each phase were discussed, highlighting the strengths and weaknesses of each approach. Tradeoffs between accuracy, computational time, and complexity were analyzed to determine the most suitable methods for the project.

## Conclusion and Future Work

In conclusion, the project developed a multi-person face recognition system from blurred images using a combination of deblurring, face detection, and face recognition techniques. Future work could involve refining the CNN architecture, exploring other deblurring methods, and addressing misclassification issues related to ethnicity.
