Python 实现人脸识别 开源

https://mp.weixin.qq.com/s?__biz=MzA4NzE1NzYyMw==&mid=2247494646&idx=2&sn=5d56f5b9af2949b856419e7ba8638d46&chksm=903f15eea7489cf8bd7ab2d5fa727ddd5f8496769fc42fb13223dfa3e2265ae8ba53b32fcb15&mpshare=1&scene=1&srcid=1029hXNxIFR3e7YGHB6LN5bn&pass_ticket=aM7AuGraBJxgAppA33wExEOMY4X0CogQeBczmgVj5HI%3D#rd

## SeetaFace Engine  

[![License](https://img.shields.io/badge/license-BSD-blue.svg)](LICENSE)

### Description

**SeetaFace Engine** is an open source C++ face recognition engine, which can run on CPU with no third-party dependence. It contains three key parts, i.e., **SeetaFace Detection**, **SeetaFace Alignment** and **SeetaFace Identification**, which are necessary and sufficient for building a real-world face recognition applicaiton system. 

* SeetaFace Detection implements a funnel-structured (FuSt) cascade schema for real-time multi-view face detection, which achieves a good trade-off between detection accuracy and speed. State of the art accuracy can be achieved on the public dataset [FDDB](http://vis-www.cs.umass.edu/fddb/) in high speed. See [SeetaFace Detection](https://github.com/seetaface/SeetaFaceEngine/tree/master/FaceDetection) for more details. 

* SeetaFace Alignment cascades several stacked auto-encoder networks to detect landmarks in real time (more than 200 fps on a single I7 desktop CPU), and achieves the state-of-the-art accuracy at least on some public datasets [AFLW](http://lrs.icg.tugraz.at/research/aflw/). See [SeetaFace Alignment](https://github.com/seetaface/SeetaFaceEngine/tree/master/FaceAlignment) for more details. 

* SeetaFace Identification is a modification of AlexNet CNN for face recognition, with better performance in terms of both accuracy (97.1% on [LFW] (http://vis-www.cs.umass.edu/lfw/) and speed (about 120ms on a single I7 desktop CPU). See [SeetaFace Identification](https://github.com/seetaface/SeetaFaceEngine/tree/master/FaceIdentification) for more details. 

This face recognition engine is developed by Visual Information Processing and Learning (VIPL) group, Institute of Computing Technology, Chinese Academy of Sciences. The codes are written in C++ without dependence on any 3rd-party libraries. The open source is now released under BSD-2 license (see [LICENSE](LICENSE) for details), which means the codes can be used freely for both acedemic purpose and industrial products.

If you meet problems when using SeetaFace Engine, you may seek help from [Configuration Documentation](./SeetaFace_config.docx).

### Contact Info

If you have any problem on SeetaFace Engine, please contact us by sending email to SeetaFace@vipl.ict.ac.cn.
If Seetaface can not meet your business needs, please contact business@seetatech.com for business cooperation. For more AI services, please visit SeetaTech official website: http://www.seetatech.com.

SeetaTech is a start-up company with the focus on computer vision technology, whose founding team comes from Visual Information Processing and Learning (VIPL) group, Institute of Computing Technology, Chinese Academy of Sciences. We have always been adhering to the development principle of "open source striving to develop AI", promoting the rapid integration of Artificial Intelligence and other industries.

### Other Documentation

* [SeetaFace Detection](./FaceDetection/README.md)
* [SeetaFace Alignment](./FaceAlignment/README.md)
* [SeetaFace Identification](./FaceIdentification/README.md)
