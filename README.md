# Image Segmentation For Unity
## Table of contents
* [General info](#general-info)
* [Requirements](#requirements)
* [Setup](#setup)
* [Details](#details)
* [Acknowledgements](#acknowledgements)

## General info
TFlite models are not totally supported in unity yet. This project allows you to use a pre-trained TFlite model for image segmentation in unity.

## Requirements
Project is created with:
* Python version: 3.6+ 64-bit
* Unity version: 2020.1+
* TensorflowLite4Unity (see https://github.com/asus4/tf-lite-unity-sample)

## Setup
To run this project,
1. Clone this repository.
2. Open project in Unity.
3. Put your tflite model in StreamingAssets folder.
4. Set the model via selecting Segmentation Manager in the scene, then choosing Model File in SelfieSegmentationSample>Options>Model File.
5. Set the color for each label via Data>OutputData.
6. Hit Play and see the results.

P.S. It is possible that you must change the model input output or its pixel painting order scrip in order to make it work properly. You can access them in `SelfieSegmentation.cs` file.

## Details
Model Output with some information about each element:
![output](https://user-images.githubusercontent.com/45734322/191551995-1b741645-c3c5-4478-a93b-2e41b3e50c5b.png)

## Acknowledgements
- This project was based on one of sample projects in [TensorflowLite4Unity](https://github.com/bkunters/TFLite4Unity) repo.
