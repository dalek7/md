# CUDA 

## Installation
```
wget http://developer.nvidia.com/compute/cuda/8.0/prod/local_installers/cuda-repo-ubuntu1404-8-0-local_8.0.44-1_amd64-deb --no-check-certificate
lspci | grep -i nvidia
sudo apt-get install linux-headers-$(uname -r)
chmod +x cuda-repo-ubuntu1404-8-0-local_8.0.44-1_amd64-deb
sudo dpkg -i cuda-repo-ubuntu1404-8-0-local_8.0.44-1_amd64-deb
sudo apt-get update
sudo apt-get install cuda
```
  
then reboot !
  
## version check
$ cat /usr/local/cuda/version.txt
$ nvcc --version

## configuration
export PATH=/usr/local/cuda-8.0/bin:$PATH
export LD_LIBRARY_PATH=/usr/local/cuda-8.0/lib64:$LD_LIBRARY_PATH
export CUDA_HOME=/usr/local/cuda-8.0/

## download links
* https://developer.nvidia.com/compute/cuda/8.0/prod/local_installers/cuda-repo-ubuntu1404-8-0-local_8.0.44-1_amd64-deb
* wget http://developer.nvidia.com/compute/cuda/8.0/prod/local_installers/cuda-repo-ubuntu1404-8-0-local_8.0.44-1_amd64-deb --no-check-certificate

## Test
- samples/1_Utilities/deviceQuery

## Helloworld
- http://computer-graphics.se/hello-world-for-cuda.html
- https://devblogs.nvidia.com/parallelforall/easy-introduction-cuda-c-and-c/
- http://blog.daum.net/heoly/7 9x9
- build
  nvcc -o saxpy saxpy.cu

## Reference
- http://haanjack.github.io/cuda/2016-02-29-cuda-linux/

