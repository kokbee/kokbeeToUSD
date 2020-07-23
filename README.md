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

