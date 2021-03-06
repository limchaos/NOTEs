# HorizonNet TF Version

At the beginning,  the TF2 re-implementation of [HorizonNet ](https://github.com/sunset1995/HorizonNet) is aimed to deploy  network of `.tflite` format to mobile devices. I therefore suggest you should first be familiar with the original implementation and paper, since deploying this network to mobile devices was temporarily paused. We currently decide to caculate layout from backend servers, so the original reponsitory should be enough for your initial work.

## Requirments

Requirments is the same as the original one, except we use tensorflow2 instead of pytorch.

## Project Location

`/media/evan/6cda00cb-e39e-4433-8097-8af7c91757a7/home/limchaos/PycharmProjects/HorizonNet_TF`

## How to trian
I use the same framework from the original reponsitory, the configuration should be the same, Run:

`python train.py --id {your ckpt id}`

network weights would be dumped in `training_checkpoints/{your ckpt id}`

## How to test

Run:

`bash run.sh`

as I said I used the same configuration as the original one, it is almost the same command to run it.

