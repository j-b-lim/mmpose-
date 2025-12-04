# Get Started

## **Environment**
- python >= 3.8.0
- pytorch >= 2.1
- CUDA 12.1+

## **Installation**

a. Create a conda virtual environment and activate it.

```shell
conda create -n MMPOSE python=3.8 -y
conda activate MMPOSE
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

e. Install mmdet.
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
The pre-trained model can be found [here](https://github.com/ultralytics/yolov5). You can test the model by running the command below.

```shell
python socket_server.py
python client.py
# Please run socket_server.py and client.py in separate terminal windows.
# Make sure to start socket_server.py before running client.py.
```

If you have any questions, please feel free to contact the writer at rkfakehd112@gmail.com.

## **References**

I referenced the repo below for the code.
- [YOLOv5](https://github.com/ultralytics/yolov5).
