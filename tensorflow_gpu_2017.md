## Tensorflow GPU
* 2017년 기준
* cudnn-8.0/cuda-8.0 + tensorflow 1.4

## CUDA Installation
* see cuda.md

## cuDNN
```
tar -zxvf cudnn-8.0-linux-x64-v5.1.tgz 
sudo cp -i lib64/libcudnn* /usr/local/cuda-8.0/lib64
sudo cp -i include/cudnn.h /usr/local/cuda-8.0/include
```
https://kusemanohar.wordpress.com/2016/06/17/installing-cudnn-ubuntu-14-04/

## Tensorflow installation
```
pip install --trusted-host pypi.python.org --upgrade tensorflow-gpu
pip install --trusted-host pypi.python.org cryptography==1.4
```
