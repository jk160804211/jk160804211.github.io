---
layout: category
titile: opencv
---
###opencv for python
*1 ####安装方法（windows下面） 
http://blog.csdn.net/qq_14845119/article/details/52354394
*2 将含有随机字节的bytearray转换为灰度图像和BGR图像：
```
import cv2
import numpy
import os

randomByteArray = bytearray(os.urandom(12000))
flatNumpyArray = numpy.array(randomByteArray)
grayImage = flatNumpyArray.reshape(300,400)
cv2.imwrite('RandomGray.png',grayImage)
bgrImage = faltNumpyArray.reshape(100,400,3)
cv2.imwrite('RandomColor.png',bgImage)
```
如果你运行该脚本，会随及生成两个图像，位于脚本所在的目录下面