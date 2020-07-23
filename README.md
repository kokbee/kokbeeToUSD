# Build To Pixar USD 

### Information
   Pixar USD 개인 빌드 레포지터리 (v0.20 >=) 

#### 1. Build info
|      Version     |   Build OS  |   Cmake  |  Gcc/G++ |   Boost  | Python2.7 |  Python3  |
|:----------------:|:-----------:|:--------:|:--------:|:--------:|:---------:|:---------:|
|      v20.08      | CentOS 7.5  | v3.13.1  |  v7.3.1  |  v1.61.0 |  v2.7.5   |     X     |
|      v20.05      | CentOS 7.5  | v3.13.1  |  v7.3.1  |  v1.61.0 |  v2.7.5   |     X     |
|      v20.02      | CentOS 7.2  | v2.8.12  |  v4.8.5  |  v1.61.0 |  v2.7.5   |     X     |

* Pixar's official github page https://github.com/PixarAnimationStudios/USD
* Read more about Pixar's USD [openusd](http://openusd.org)


#### 2. Build Command
|      Version     | Command |
|:----------------:|:--------------------------------------------------------------------------------------------------:|
|      v20.08      | python USD/build_scripts/build_usd.py --openimageio --opencolorio --ptex --alembic /usr/local/USD  |
|      v20.05      | python USD/build_scripts/build_usd.py --openimageio --opencolorio --ptex --alembic /usr/local/USD  |
|      v20.02      | python USD/build_scripts/build_usd.py --openimageio --opencolorio --ptex --alembic /usr/local/USD  |

#### 3. Thrid Party Command
|      Version     | Maya Command |
|:----------------:|:------------------------------------------------------------------------------------------------------------:|
|      v20.02      | python build.py --maya-location /usr/autodesk/maya20XX --pxrusd-location /usr/local/USD /usr/local/workspace |

* Autodesk Maya official github page https://github.com/Autodesk/maya-usd
* The documentation that was previously on this page can be found at [maya-usd](https://github.com/Autodesk/maya-usd/blob/dev/plugin/pxr/doc/README.md)

#### 4. Use USD & Environment Setup
   1. tar -zxvf v20.xx.tar.gz 
   2. cp -rf USD /usr/local/USD
   3. export PYTHONPATH=/usr/local/USD/lib/python:$PYTHONPATH
   4. export PATH=/usr/local/USD/bin:$PATH

### Run Python USD
* from pxr import Usd

### Etc & Build Tip
* USD core만 빌드된 레포지터리입니다.
* python USD/build_scripts/build_usd.py -v -v 옵션을 주면 컴파일 진행 상황을 볼 수 있습니다.
* 우분투와 CentOS8에서 빌드 가능합니다.
* 서드파티 플러그인은 v0.19버전까지 core 스크립트로만 가능합니다.
