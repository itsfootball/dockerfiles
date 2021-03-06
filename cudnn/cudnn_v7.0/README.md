[![Docker Pulls](https://img.shields.io/docker/pulls/kaixhin/cudnn.svg)](https://hub.docker.com/r/kaixhin/cudnn/)
[![Docker Stars](https://img.shields.io/docker/stars/kaixhin/cudnn.svg)](https://hub.docker.com/r/kaixhin/cudnn/)

cudnn
=====
**DEPRECATED:** Please use [NVIDIA Docker](https://github.com/NVIDIA/nvidia-docker).

Ubuntu Core 14.04 + [CUDA 7.0.28](http://www.nvidia.com/object/cuda_home_new.html) + [cuDNN v4](https://developer.nvidia.com/cuDNN).

Requirements
------------

- Host with corresponding CUDA drivers (v. 346.46) installed for the kernel module.

Usage
-----
The container must have all NVIDIA devices attached to it for CUDA to work properly.
Therefore the command will be as such: `docker run -it --device /dev/nvidiactl --device /dev/nvidia-uvm --device /dev/nvidia0 kaixhin/cudnn`.
With 4 GPUs this would also have to include `--device /dev/nvidia1 --device /dev/nvidia2 --device /dev/nvidia3`.

For more information on CUDA on Docker, see the [repo readme](https://github.com/Kaixhin/dockerfiles#cuda).

Citation
--------
If you find this useful in research please consider [citing this work](https://github.com/Kaixhin/dockerfiles/blob/master/CITATION.md).
