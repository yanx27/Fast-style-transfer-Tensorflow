# Neural Style Transfer

## Reference
[Perceptual Losses for Real-Time Style Transfer and Super-Resolution](https://arxiv.org/abs/1603.08155) <br> 
## Data
* VOC2014<br> 	
[here](http://msvocds.blob.core.windows.net/coco2014/train2014.zip)  <br> 
* Pretrain VGG-19<br> 
[here](http://www.vlfeat.org/matconvnet/models/beta16/imagenet-vgg-verydeep-19.mat)  <br> 

Download them and put in `./data`<br> 
## Training
```
python style.py --checkpoint ./model --style ./style/xxx.jpg 
```
## Evaluation
```
python evaluate.py --checkpoint ./model/xxx --in-path ./examples/content/xxx.jpg --out-path ./
```

## Results
![](https://github.com/yanx27/Fast-style-transfer-based-on-Tensorflow/blob/master/examples/results/sysu.jpg)  

