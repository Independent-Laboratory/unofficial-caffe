# [Unofficial] Caffe for 2021 latest environment (For Ubuntu 20.04.2 LTS 64 bit, RTX3080, CUDA 11.1, cDNN 8.2.0, python 3.8.0, opencv 4.2.0)

This is unofficial modified version of Caffe 1.0.0 supporting 2021 latest environment.
The original repository is https://github.com/BVLC/caffe

The modification is trivial fix and not version up.
This is mainly for my memorandum record, however, it is OK to use this if you like this fix. 
And if you are familiar with opensource community work and good at English conversation, it is welcome that you propose this modification to official repository instead of me (but I can not have responsibility, sorry).

## Modified parts
Main modification is for supporting OpenCV 4.
I made an example of "Makefile.config" based on "Makefile.config.Makefile.config.example".
And I add trivial fix in some source code.

## Prepare for installation
```
sudo apt install libboost-dev 
sudo apt install libgflags-dev
sudo apt install libatlas-base-dev
sudo apt install libhdf5-dev
sudo apt install libblas-dev
sudo apt install libatlas-base-dev
sudo apt install libsnappy-dev
```

This instruction is from my memory and there might be some forgotten installation.

## Install and test
```
$ make -j8
$ make test -j8
$ make 
```
Some warning is shown, however, run test was passed on my machine.
So, Caffe might run appropriately also in practical use.

## License
License and Copyright are same as original repository (https://github.com/BVLC/caffe).
The same license file is attached on this repository as "LICENSE" file.

In the case of I make license violation on this repository, I will fix or delete this repository quickly.