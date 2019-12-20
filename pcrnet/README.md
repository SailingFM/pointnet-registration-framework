# Point Cloud Registration Network

Source Code Author: Vinit Sarode, Xueqian Li and Animesh Dhagat

### Dataset:
Path for dataset: [Link](https://drive.google.com/drive/folders/19X68JeiXdeZgFp3cuCVpac4aLLw4StHZ?usp=sharing)
1. Download 'train_data' folder from above link for iterative PCRNet.
2. Download 'car_data' folder from above link for PCRNet.

### Pretrained Model:
Download pretrained models from [Link](https://drive.google.com/drive/folders/1o3F6677n6FVuMArNVWTyP5Hn3m856eEG?usp=sharing)

### How to use code:

#### Compile loss functions:
1. cd utils/pc_distance
2. make -f makefile_10.0 clean
3. make -f makefile_10.0

#### Train Iterative-PCRNet:
1. chmod +x train_itrPCRNet.sh
2. ./train_itrPCRNet.sh

#### Train PCRNet:
1. chmod +x train_PCRNet.sh
2. ./train_PCRNet.sh

#### Train Partial PCRNet:
1. python iterative_PCRNet_partial.py --mode train --log log_partial --use_noise_data True