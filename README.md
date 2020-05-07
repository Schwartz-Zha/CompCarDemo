# This is a demo Car Classification Project running on CompCar dataset with Resnet50 architecture

## Required Libraries
torch, torchvision, PIL, scipy, matplotlib

## Dataset Description

The CompCar dataste is provided here http://mmlab.ie.cuhk.edu.hk/datasets/comp_cars/index.html

It's ecpteced to download and upzip the whole dataset under PROJECT_ROOT/Dataset.

Meanwhile, there is also a file called "full_model_name_updated.txt" under PROJECT_ROOT?Dataset, while contains 136725 lines. Each line will map a image file's directory (used to 
load this image) to the actual car model label.

## Model Description
Directly use the implementation in torchvision for resnet50.

The pretrained model should be downloaded [here](https://drive.google.com/file/d/12GewzNMJmmUqvumDogm7m16ewxRKqCLS/view?usp=sharing), and put into 
PROJECT_ROOT/Code/checkpoint2/10_epoch.tar 

## Code
All the codes are push onto this repository, but the final one with full annotations is PROJECT_ROOT/Code/CarClassificationDemo2.ipynb

All the other codes are not for demonstration purpose.
