# MEGADOCK 4.0

**MEGADOCK 4.0** is a structural bioinformatics software for FFT-grid-based protein-protein docking that takes advantage of the massively parallel CUDA architechture of NVIDIA GPUs and multiple computation nodes.  
[http://www.bi.cs.titech.ac.jp/megadock/](http://www.bi.cs.titech.ac.jp/megadock/)

[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](LICENSE)
[![Build Status](https://travis-ci.org/akiyamalab/MEGADOCK.svg?branch=master)](https://travis-ci.org/akiyamalab/MEGADOCK)


## Target Environments
| Type | Environment     | Parallelization   |
|:----:|-----------------|-------------------|
|  (a) | GPU cluster     | GPU, MPI + OpenMP |
|  (b) | CPU cluster     | MPI + OpenMP      |
|  (c) | GPU single node | GPU               |
|  (d) | CPU single node | OpenMP            |

## Requirements
| Libraries                                                       | GPU cluster | CPU cluster | GPU | CPU | Notes |
|:----------------------------------------------------------------|:-----------:|:-----------:|:---:|:---:|:------|
| [FFTW3](http://www.fftw.org)                                    | x           | x           | x   | x   | `--enable-float` flag required (see [FAQ](http://www.bi.cs.titech.ac.jp/megadock/faq.html))|
| [OpenMPI](http://www.open-mpi.org)                              | x           | x           |     |     |       |
| [CUDA Toolkit](https://developer.nvidia.com/cuda-zone)          | x           |             | x   |     | `ver >= 5.0` required |
| [CUDA SDK code samples](https://developer.nvidia.com/cuda-zone) | x           |             | x   |     | **same version as CUDA Toolkit** |

## Installation
Please refer to the following documents and see the appropriate instructions for your environment.  
* [doc/BUILD.md](./doc/BUILD.md)
* [doc/README.md](./doc/README.md)

### MEGADOCK in Docker Container
[Dockerfiles/README.md](Dockerfiles/README.md)


## Reference
Masahito Ohue, Takehiro Shimoda, Shuji Suzuki, Yuri Matsuzaki, Takashi Ishida, Yutaka Akiyama. MEGADOCK 4.0: an ultra-high-performance protein-protein docking software for heterogeneous supercomputers, Bioinformatics, 30(22): 3281-3283, 2014.

## Older Versions
For older versions can be downloaded from the following URL.  
[http://www.bi.cs.titech.ac.jp/megadock/archives/](http://www.bi.cs.titech.ac.jp/megadock/archives/)

## Lisence
MEGADOCK is open source licensed under the GNU General Public License, version 3 or later. 

## Fundings
This work is partially supported by JSPS Grant-in-Aid for Scientific Research (KAKENHI) (A) Grant Number 24240044.

----
Copyright © 2014-2017 Akiyama Laboratory, Tokyo Institute of Technology, All Rights Reserved.

