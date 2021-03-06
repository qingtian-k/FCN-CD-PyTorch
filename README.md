# Fully Convolutional Siamese Networks for Change Detection

This is an unofficial implementation of the paper

> Rodrigo Caye Daudt, Bertrand Le Saux, Alexandre Boulch. (2018, October). Fully convolutional siamese networks for change detection. In 2018 25th IEEE International Conference on Image Processing (ICIP) (pp. 4063-4067). IEEE.
 
as the [official repo](https://github.com/rcdaudt/fully_convolutional_change_detection) does not provide the training code. 

[paper link](https://ieeexplore.ieee.org/abstract/document/8451652)

# Basic Usage

```bash
# The network definition scripts are from the original repo
git clone --recurse-submodules git@github.com:Bobholamovic/FCN-CD-PyTorch.git   
```

For training, try

```bash
# In the root directory of this repository
mkdir exp
cd src
python train.py train --exp-config ../config_base.yaml
```

For evaluation, try

```bash
python train.py val --exp-config ../config_base.yaml --resume path_to_checkpoint
```

You can find the checkpoints in `exp/base/weights/`, the log files in `exp/base/logs`, and the output change maps in `exp/outs`.