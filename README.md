基于Tensorflow的快速图像风格迁移
====  
#
>	主要参考文献为李飞飞的《Perceptual Losses for Real-Time Style Transfer and Super-Resolution》<br> 
#
>* 训练数据，8W多 12G<br> 	
[数据链接](http://msvocds.blob.core.windows.net/coco2014/train2014.zip)  <br> 
>* 训练好的VGG-19模型<br> 
[VGG-19链接](http://www.vlfeat.org/matconvnet/models/beta16/imagenet-vgg-verydeep-19.mat)  <br> 

>把这两个文件下载好了之后放在data文件夹里<br> 
#
>训练模型：
```
python style.py --checkpoint ./model --style ./style/xxx.jpg 
```
#
>测试已有模型：（下载release中的模型并放在model文件夹里）<br> 
```
python evaluate.py --checkpoint ./model/xxx --in-path ./examples/content/xxx.jpg --out-path ./
```
>填上模型名称、图片的输入路径和输出路径
#
风格迁移效果
-------
![](https://github.com/yanx27/Fast-style-transfer-based-on-Tensorflow/blob/master/examples/results/sysu.jpg)  

