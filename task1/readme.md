# How to run
## baseline
```
python main.py dataset --gpu 0 --epochs 200 --lr 0.01 --augment none
```
## mixup
```
python main.py dataset --gpu 0 --epochs 200 --lr 0.01 --augment mixup
```
## cutout
```
python main.py dataset --gpu 0 --epochs 200 --lr 0.01 --augment cutout
```
## cutmix
```
python main.py dataset --gpu 0 --epochs 200 --lr 0.01 --augment cutmix
```
# Visualization
运行代码在visual.ipynb中

# Result & Tensorboard
模型运行结果会自动储存在results文件夹之下，运行tensorboard时需进入到对应的目标文件之下，以cutmix运行结果为例，其他运行结果只需将cutmix改成mixup等即可。
```
cd results/cutmix
tensorboard --logdir logs
```
