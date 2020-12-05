# Row web tools
一套强大的ROS，web相关功能组件, http://robotwebtools.org/index.html

demo: https://webviz.io/app/

包括ros功能包
 - rosbridge_suite
 - roslibjs
 - web_video_server
 - ...

# web_video_server实现目的
## 1 安装依赖库async-web-server
```shell
sudo apt-get install ros-kinetic-async-web-server-cpp
```

## 2 下载ros节点源码
git clone https://github.com/RobotWebTools/web_video_server

## 3 编译运行ros节点
```shell
mkdir src
mv web_video_server src/
cd …/
catkin_make
roscore
```

## 4 在web中显示效果
打开浏览器输入如下地址:
http://localhost:8080/stream?topic=/usb_cam/image_raw
此处/usb_cam/image_raw表示usb camera的rostopic节点原始数据
