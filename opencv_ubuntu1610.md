# OpenCV @Ubuntu 16.10
```
sudo apt-get install build-essential checkinstall cmake git pkg-config yasm libtiff5-dev libjpeg-dev libjasper-dev libavcodec-dev libavformat-dev libswscale-dev libdc1394-22-dev libxine2-dev libv4l-dev python-dev python-numpy libtbb-dev libgtk2.0-dev libfaac-dev libmp3lame-dev libopencore-amrnb-dev libopencore-amrwb-dev libtheora-dev libvorbis-dev libxvidcore-dev x264 v4l-utils libopenexr-dev python-tk  libeigen3-dev libx264-dev
```
```
sudo add-apt-repository ppa:mc3man/gstffmpeg-keep
sudo apt-get update
sudo apt-get install ffmpeg
```

```
git clone https://github.com/opencv/opencv.git
git clone https://github.com/opencv/opencv_contrib.git
```

```
cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local \
-D BUILD_NEW_PYTHON_SUPPORT=ON -D WITH_V4L=ON \
-D WITH_TBB=ON -D WITH_IPP=OFF \
-DOPENCV_EXTRA_MODULES_PATH=../../opencv_contrib/modules  ../ 
```
