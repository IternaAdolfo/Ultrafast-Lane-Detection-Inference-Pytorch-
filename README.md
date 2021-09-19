# Ultrafast Lane Detection Inference Pytorch
Example Jupyter-Notebook file for the detection of lanes using the [ultra fast lane detection model](https://github.com/cfzd/Ultra-Fast-Lane-Detection) in Pytorch.


Source: https://www.flickr.com/photos/32413914@N00/1475776461/
![!Ultra fast lane detection](https://github.com/ibaiGorordo/Ultrafast-Lane-Detection-Inference-Pytorch-/blob/main/doc/img/detected%20lanes.jpg)

# Requirements

 * **OpenCV**, **Scikit-learn** and **pytorch**. 

# Conda and Carla Requirements
```
# conda install pytorch torchvision torchaudio cudatoolkit=10.1 -c pytorch
# conda create --name pytorch-gpu-cuda10.1   **-c pytorch**  pytorch torchvision  cudatoolkit=10.1 jupyterlab scikit-learn opencv


cd workspace/github/Ultrafast-Lane-Detection-Inference-Pytorch-
conda info --envs
conda activate pytorch-gpu-cuda10.1
jupyter-lab

cd Downloads\CARLA_0.9.12\WindowsNoEditor
CarlaUE4 /Game/Carla/Maps/Town03 -windowed -ResX=256 -ResY=128 -carla-port=3000 -benchmark -fps=30   -quality-level=Epic
```
 
# Installation
```
pip install carla
```
**Pytorch:** Check the [Pytorch website](https://pytorch.org/) to find the best method to install Pytorch in your computer.

# Pretrained model
Download the pretrained model from the [original repository](https://github.com/cfzd/Ultra-Fast-Lane-Detection) and save it into the **[models](https://github.com/ibaiGorordo/Ultrafast-Lane-Detection-Inference-Pytorch-/tree/main/models)** folder. 

# Ultra fast lane detection - TuSimple([link](https://github.com/cfzd/Ultra-Fast-Lane-Detection))

 * **Input**: RGB image of size 1280 x 720 pixels.
 * **Output**: Keypoints for a maximum of 4 lanes (left-most lane, left lane, right lane, and right-most lane).
 
# Examples

 * **Carla RGB Cam inference**:
 
 ```
carlaLaneDetection.ipynb ```
 

 
 # [Inference video Example](https://youtu.be/0Owf6gef1Ew) 
 ![!Ultrafast lane detection on video](https://github.com/ibaiGorordo/Ultrafast-Lane-Detection-Inference-Pytorch-/blob/main/doc/img/laneDetection.gif)
 
 Original video: https://youtu.be/2CIxM7x-Clc (by Yunfei Guo)
 
