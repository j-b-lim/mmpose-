# Get Started

## **Environment**
- python >= 3.8.0
- pytorch >= 2.1
- CUDA 12.1+

## **Installation**

a. Create a conda virtual environment and activate it.

```shell
conda create -n mmpose python=3.8 -y
conda activate mmpose
```

b. Install PyTorch and torchvision following the [official instructions](https://pytorch.org/), *e.g.*,

```shell
# CUDA 12.1
conda install pytorch==2.1.0 torchvision==0.16.0 torchaudio==2.1.0 pytorch-cuda=12.1 -c pytorch -c nvidia
```

c. Install MMEngine and MMCV using MIM.
```shell
pip install -U openmim
mim install mmengine
mim install "mmcv>=2.0.0,<2.0.0"
```

e. Install MMDET.
```shell
mim install "mmdet>=3.0.0"
```

d. Install required packages
```shell
git clone https://github.com/open-mmlab/mmpose.git
cd mmpose
pip install -r requirements.txt
pip install -v -e .
```

## **Quick Start**
```shell
python demo/inferencer_demo.py $IMAGE --pose2d rtmo --vis-out-dir vis_results
```
The [RTMO](https://github.com/open-mmlab/mmpose/tree/main/projects/rtmo) model was used to complete the Quick Start.

## **References**

I referenced the repo below for the code.
- [MMPose Installation](https://mmpose.readthedocs.io/en/latest/installation.html).
- [MMPose Github](https://github.com/open-mmlab/mmpose).

- If you have any questions, please feel free to contact the writer at rkfakehd112@gmail.com.
