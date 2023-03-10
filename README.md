# CCN_PROJECT - Group 6
# Team Members
* Narasimha Naidu Kommi
* Venkata Sai Shalini Ganni
* Siva Naga Rutwik Reddy Chintha
* Prashanth Sammanu

#  Introduction
This project is to utilize Core Machine Learning to perform Object Segmentation with Face Parsing and develop a mobile application, specifically for IOS. To achieve this, we will be utilizing various models throughout the project.
## Implementation Methodology

### 1. DeepLabV3 :
A potent model for object segmentation is DeepLabV3 (https://pytorch.org/hub/pytorch_vision_deeplabv3_resnet101/ ). In object segmentation, each pixel in an image is given a label indicating what object or class it pertains to. It can be used in a wide variety of real-world situations, such as autonomous driving, medical imaging, and picture editing.

We want to use various extensions to DeepLabV3, such as DeepLabV3FP1 is an extension of the original DeepLabV3 architecture. It incorporates a feature pyramid network (FPN) that allows the model to more effectively capture and integrate features at multiple scales.  This allows the model to more effectively integrate features across different scales, which can be important for accurately segmenting objects in images. And we also would like to use DeepLabV3Int8LUT is a variant of the DeepLabV3 image segmentation model that uses an 8-bit integer look-up table (LUT) for efficient inference on low-power devices.

DeepLabV3Int8LUT is particularly well-suited for use on mobile and embedded devices with limited processing power and memory, where it can provide real-time segmentation of images. The model is trained in the same way as the original DeepLabV3 model, but during inference, the pre-computed LUTs are used to speed up the calculations and reduce memory usage.

We want to compare the inferences between different flavours of this model and show the inference and execution time, even on both CPU and GPU. 

### 2. Face Parsing :

Face Parsing is a computer vision technique that involves segmenting a human face into different regions or parts, each corresponding to a different facial feature, such as the eyes, nose, mouth, cheeks, and forehead. This can be useful for a range of applications, including face recognition, facial expression analysis, and virtual makeup and accessories.

Face Parsing typically involves training a deep learning model on a large dataset of labelled images, where each pixel in the image is labeled according to the corresponding facial feature. The model can then be used to predict the facial feature segmentation for new images.

The output of a Face Parsing model is usually a color-coded mask, where each facial feature is represented by a different colour. This can be overlaid on the original image to visualize the segmentation. Face Parsing is a challenging problem due to the large variability in facial appearance across individuals, lighting conditions, and poses, but recent advances in deep learning have led to significant improvements in performance.


### 3. IOS Mobile Application :

Our mobile application project will include a range of features, such as the ability to select images from the device's gallery, as well as capturing live images using the device's camera application. One of the primary features we plan to implement is segmentation parsing.

A computer vision task known as object segmentation entails dividing an image into a number of segments, each of which correlates to a different object or area within the image. Identifying and separating each object in an image from its backdrop is the aim of object segmentation.

We aim to **emphasize real-time recording and inference in our project, to enable users to see the process of the app analyzing and parsing the images in real-time**. Our goal is to demonstrate how the inference process works and how it helps in segmenting and parsing images. And compare them real time. 


# Architecture

## Architecture Diagram:

![Screenshot](architecture.png)

## Pytorch to CoreML Coversion:

![Screenshot](pytorch_to_coreml.png)

# Project Plan based on two weeks iteration
## Iteration 1
* Gather requirements for the project,Define project scope and objectives. Set up project repository on GitHub and add team members as collaborators
* Familiarize with the technologies and the concepts.
* Divide the project into small parts and assign to each member.
* Set up the environment required to run the model.
* Develop the app interface using Apple's Xcode IDE.
* Implement the interface for the app's camera feature and integrate image capture and storage capabilities. Implement basic image processing functions to convert images to input format required by the segmentation model.
## Iteration 2
* Individual assignment Of each Team memeber to be determined
* Perform preliminary testing of the model to assess its precision and pinpoint opportunities for enhancement.
* Modifying the model as required to boost its precision.
* Validating the complete functionality of the model to guarantee that it satisfies the project specifications.
* Add Video capture and support DeepLabV3 model on LiveImageViewController.
* Predict an image imported from our device???s photo library. Configuring Colour range. 
* Adding Inference time in the mobile application. 
## Iteration 3
* Expand the segmentation model.
* CImplement segmentation features for the additional facial features
* IImprove the app's user interface and usability. Add gpu in the mobile application.
* Examine the system's complete operation and, in the event of any problems, troubleshoot and eliminate them to guarantee the application operates seamlessly.
## Iteration 4
* Implement real-time video segmentation and integrate it with the camera feature..
* Optimize the app's performance and memory usage. Support face parsing and object segmentation model.
* Adding app tab item and page for tracking face and segmenting it. 
* If issues are found, analyze the root cause and take necessary actions to resolve them.
## Iteration 5
* Get the project documentation ready.
* Construct the presentation and present the completed project.