# Super Tiger AI Printer 1.2.1
## Artificial intelligence printer, **REAL** time image recognition.

>Written by **张春哲** with love.
>Contact: [sepmein@gmail.com](sepmein@gmail.com)

## 1. HardWare and Frameworks
### 1.1 Realtime image recognition framework

![tensorflow](https://camo.githubusercontent.com/aeb4f612bd9b40d81c62fcbebd6db44a5d4344b8b962be0138817e18c9c06963/68747470733a2f2f7777772e74656e736f72666c6f772e6f72672f696d616765732f74665f6c6f676f5f686f72697a6f6e74616c2e706e67)

This framework used full CNN 

#### Convolutional Neural Network

![CNN](https://www.researchgate.net/profile/Thorsten-Hoeser/publication/341576780/figure/fig2/AS:894032699998208@1590165414024/Overview-and-details-of-a-convolutional-neural-network-CNN-architecture-for-image.ppm)

### 1.2 SnapMaker 2.0
![SnapMaker](http://www.3dtoutiao.com/uploads/allimg/200608/1-20060Q64ZKM.png)

### 1.3 RasperryPI 4.0 Pro
![Rasperry](https://upload.wikimedia.org/wikipedia/commons/d/d1/Raspberry_Pi_OS_Logo.png)

## 2. Install and Usage

### 2.1 Getting started
See the install guide for the pip package, to enable GPU support, use a Docker container, and build from source.

To install the current release, which includes support for CUDA-enabled GPU cards (Ubuntu and Windows):

```terminal
$ pip install tiger-printer
```

### 2.2 Basic Usage
Run the following code in your terminal
```terminal
$ echo -e "\e[1;40m" ; clear ; while :; do echo $LINES $COLUMNS $(( $RANDOM % $COLUMNS)) $(( $RANDOM % 72 )) ;sleep 0.05; done|awk '{ letters="abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789@#$%^&*()"; c=$4; letter=substr(letters,c,1);a[$3]=0;for (x in a) {o=a[x];a[x]=a[x]+1; printf "\033[%s;%sH\033[2;32m%s",o,x,letter; printf "\033[%s;%sH\033[1;37m%s\033[0;0H",a[x],x,letter;if (a[x] >= $1) { a[x]=0; } }}'
```
