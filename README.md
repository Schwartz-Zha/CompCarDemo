# This is a demo Car Classification Project running on CompCar dataset with Resnet50 architecture

## Required Libraries
torch, torchvision, PIL, scipy, matplotlib

## Dataset Description

The CompCar dataste is provided here http://mmlab.ie.cuhk.edu.hk/datasets/comp_cars/index.html

It's inherited from the work of "Linjie Yang, Ping Luo, Chen Change Loy, Xiaoou Tang. A Large-Scale Car Dataset for 
Fine-Grained Categorization and Verification, In Computer Vision and Pattern Recognition (CVPR), 2015."

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

## How to use this demo

(1) Download and extract the dataset [here](http://mmlab.ie.cuhk.edu.hk/datasets/comp_cars/instruction.txt).

(2) Download this project. And put the dataset just downloaded into PROJECT_ROOT/Dataset/. An image in thid 
dataset should look like this CompCarDemo/Dataset/data/image/1/1101/2011/07b90decb92ba6.jpg

(3) This project is built with jupyter notebook and several scientific packages of python. So it's highly 
recommended to use anaconda to manage all these required packages in one place. Futhermore, miniconda is a much 
more lighweighted version, which takes much smaller space than Anaconda. It could be downloaded 
[here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/).

(4) After installing the anaconda, the command 'conda' should be available in the terminal. The discription below is 
provided for Mac/Linux command line interface, simply because I'm unfamiliar with Windows termimal.

```shell
conda create --name CompCarDemoEnv python=3.6 #create a new environment in case the default python version is 2.x
conda activate CompCarDemoEnv #enter the new environment
conda install jupyter #for installing jupyter notebook

#use this line if you have a CUDA accelerated GPU
conda install pytorch torchvision cudatoolkit=10.2 -c pytorch

#use this line if not
conda install pytorch torchvision

conda install PIL,scipy,matplotlib
```
(5) Download the pretrained model [here](https://drive.google.com/file/d/12GewzNMJmmUqvumDogm7m16ewxRKqCLS/view), 
and put it like CompCarDemo/Code/checkpoint2/10_epoch.tar


(6) It's time to see the demo.

```shell
jupyter notebook
```
Then open the file CompCarDemo/Code/CarClassificationDemo2.ipynb in the browser interface. Ready to go.
