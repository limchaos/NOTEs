# Neural style transfer 

## Project location

`/media/evan/6cda00cb-e39e-4433-8097-8af7c91757a7/home/limchaos/PycharmProjects/neural-style-pytorch`

## Dataset

The dataset I used for tiaining is [COCO2014](http://cocodataset.org/#download), which is about 13GB, make sure you download it with enough storage.

## How to train

If your want to visulize your training , first open the ** visdom sever** by running  `python -m visdom.server` 

<img src="/home/evan/README/imgs/visdom.png" width="650">

 then access  default address `http://localhost:8097`from your browser.

Simply  run :

` python train  --data_path  {path to training dataset} --model_name  {custom name} --style_path {path to your style image}`

There are some examples you could find from `train.sh`,  generated checkpoints could be found from ** ./checkpoint**.

<img src="/home/evan/README/imgs/vis.png" width="650">

You could find more detailed  configuration  from  `config.py`, such as `learning rate, style weight or vgg features, etc`.



## How to test

Run :

`python inference.py --model_path {your model path} --input_path {path to your content image} --output_path {output path}`

Some examples could be found from `test.sh`, run `./test.sh` to have a look.

## co-workers 

Usually, you only need to contact

![](/home/evan/README/imgs/jinran.png) 

and send him the new `.pth` model.