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
![img text](http://github.com/JCPLiang/HPML_Project/raw/master/img/dali_time.png)
## Network Refining
The three
