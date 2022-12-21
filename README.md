# HPML_Project

## NVIDIA Dali
This is a tool to speed up data loading. Begin the experiment by:
```
python miniGooglenet_dali.py
```
Need to install and meet the requirements of cuda version for dali before running.
```
pip install --extra-index-url https://developer.download.nvidia.com/compute/redist --upgrade nvidia-dali-tf-plugin-cuda102
pip install --extra-index-url https://developer.download.nvidia.com/compute/redist/nightly --upgrade nvidia-dali-nightly-cuda102
pip install --extra-index-url https://developer.download.nvidia.com/compute/redist/nightly --upgrade nvidia-dali-tf-plugin-nightly-cuda102
```
There will be a great improvement using Dali compared to dataloader in Pytorch.
<img src="https://github.com/JCPLiang/HPML_Project/blob/main/img/dali_time.PNG" width="450" height="300">
## Network Refining
There are three versions of miniGooglenet. Begin the experiment by:
```
python miniGooglenet.py
```
<img src="https://github.com/JCPLiang/HPML_Project/blob/main/img/mini_acc.PNG" width="350" height="280">
<img src="https://github.com/JCPLiang/HPML_Project/blob/main/img/mini_time.PNG" width="380" height="280">

## Pretrain Resnet
Because of the remaining connections in Resnet, we can pre-train part of Resnet to speed up the convergence of the whole net. Begin the experiment by:
```
python Resnet34_pretrain.py
```
<img src="https://github.com/JCPLiang/HPML_Project/blob/main/img/train_acc.PNG" width="350" height="280">
<img src="https://github.com/JCPLiang/HPML_Project/blob/main/img/test_acc.PNG" width="340" height="280">

