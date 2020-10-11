## Acuity Model Zoo

Acuity model zoo contains a set of popular neural-network models created or converted (from Caffe, Tensorflow, TFLite, DarkNet or ONNX) by Acuity toolset.

### Model Viewer
Acuity uses JSON format to describe a neural-network model, and we provide an [online model viewer](https://verisilicon.github.io/acuity-models/viewer/index.html) to help visualized data flow graphs. The model viewer is inspired by [netron](https://github.com/lutzroeder/netron).

### Classification
 - [Alexnet][]([OriginModel][OriginAlexnet])
 - [Inception-v1][] ([OriginModel][OriginInception-v1])
 - [Inception-v2][] ([OriginModel][OriginInception-v2])
 - [Inception-v3][] ([OriginModel][OriginInception-v3])
 - [Inception-v4][] ([OriginModel][OriginInception-v4])
 - [Mobilenet-v1][] ([OriginModel][OriginMobilenet-v1])
 - [Mobilenet-v2][] ([OriginModel][OriginMobilenet-v2])
 - [Mobilenet-v3][] ([OriginModel][OriginMobilenet-v3])
 - [EfficientNet][] ([OriginModel][OriginEfficientNet])
 - [EfficientNet (EdgeTPU)][] ([OriginModel][OriginEfficientNet-EdgeTPU])
 - [Nasnet-Large][] ([OriginModel][OriginNasnet-Large])
 - [Nasnet-Mobile][] ([OriginModel][OriginNasnet-Mobile])
 - [Resnet-50][] ([OriginModel][OriginResnet-50])
 - [Resnext-50][] ([OriginModel][OriginResnext-50])
 - [Senet-50][] ([OriginModel][OriginSenet-50])
 - [Squeezenet][] ([OriginModel][OriginSqueezenet])
 - [VGG-16][] ([OriginModel][OriginVGG-16])
 - [Xception][] ([OriginModel][OriginXception])

### Detection
 - [Faster-RCNN-ZF][] ([OriginModel][OriginFaster-RCNN-ZF])
 - [Mobilenet-SSD][] ([OriginModel][OriginMobilenet-SSD])
 - [Mobilenet-SSD-FPN][] ([OriginModel][OriginMobilenet-SSD-FPN])
 - [MTCNN PNet][]([OriginModel][OriginMTCNN PNet]) [RNet][]([OriginModel][OriginRNet]) [ONet][]([OriginModel][OriginONet]) [LNet][]([OriginModel][OriginLNet])
 - [SSD][] ([OriginModel][OriginSSD])
 - [Tiny-YOLO][] ([OriginModel][OriginTiny-YOLO])
 - [YOLO-v1][] ([OriginModel][OriginYOLO-v1])
 - [YOLO-v2][] ([OriginModel][OriginYOLO-v2])
 - [YOLO-v3][] ([OriginModel][OriginYOLO-v3])

### Segmentation
 - [ENET][] ([OriginModel][OriginENET])
 - [SegNet][] ([OriginModel][OriginSegNet])
 - [DeepLab-v3][] ([OriginModel][OriginDeepLab-v3])

### Pixel Processing
 - [Denoiser][] 
 - [Super Resolution][] ([OriginModel][OriginSuper Resolution])
 - [Fast Style Transfer][] ([OriginModel][OriginFast Style Transfer])
 - [Pix2Pix][] ([OriginModel][OriginPix2Pix])

### Pose Estimation
 - [Open Pose][] ([OriginModel][OriginOpen Pose])
 - [CPM Mobile][] ([OriginModel][OriginCPM Mobile])

### Recurrent Net
 - [LSTM - Command Recognition][]
 - [LSTM - Speech Recognition][]

## About Acuity

Acuity is a python based neural-network framework built on top of Tensorflow, it provides a set of easy to use high level layer API as well as infrastructure for optimizing neural networks for deployment on [Vivante Neural Network Processor IP](http://www.verisilicon.com/en/IPPortfolio/VivanteNPUIP) powered hardware platforms. Going from a pre-trained model to hardware inferencing can be as simple as 3 automated steps.

![Acuity Workflow](/docs/acuity_123.png)


 - Importing from popular frameworks such as Tensorflow and PyTorch

   > AcuityNet natively supports Caffe, Tensorflow, PyTorch, ONNX, TFLite, DarkNet, and Keras imports, it can also be expanded to support other NN frameworks.  

 - Fixed Point Quantization

   > AcuityNet provides accurate Post Training Quantization and produces accuracy numbers before and after quantization for comparison. Advanced techniques are built-in into AcuityNet quantizer, such as KL-Divergence, Weight Equalization, Hybrid Quantization, Per Channel Quantization, etc.

 - Graph Optimization  

   > Neural-network graph optimization is performed to reduce graph complexity for inference, such as Layer Fusion, Layer Removal and Layer Swapping  

 - Tensor Pruning  

   > Pruning neural networks tensors to remove ineffective synapses and neurons to create sparse matrix  

 - Training and Validation  

   > AcuityNet provides capability to train and validate Neural Networks

 - Inference Code Generator  

   > Generates OpenVX Neural Network inference code which can run on any OpenVX enabled platforms  

## About Vivante NPUIP

Vivante NPUIP is a highly scalable and programmable neural network processor that supports a wide range of Machine Learning applications. It has been deployed in many fields to accelerate ML algorithms for AI-vision, AI-voice, AI-pixel and other special use cases. Vivante NPUIP offers high performance MAC engine as well as flexible programmable capability to adopt new operations and networks without having to fall back to CPU. Today, over 120 operators are supported and continue to grow.

Mature software stack and complete solutions are provided to customers for easy integration and fast time to market. 

Tooling
 - Acuity Toolkits
 - Acuity IDE

Runtime software stack support
 - OpenVX and OpenVX NN Extension
 - OpenCL
 - Android NN API
 - TFLite NPU Delegate
 - ONNX Runtime Execution Provider
 - ARMNN Backend

[Alexnet]: https://hawk081.github.io/acuity-models/viewer/?url=../models/alexnet/alexnet.json
[Inception-v1]: https://hawk081.github.io/acuity-models/viewer/?url=../models/inception_v1/inception_v1.json
[Inception-v2]: https://hawk081.github.io/acuity-models/viewer/?url=../models/inception_v2/inception_v2.json
[Inception-v3]: https://hawk081.github.io/acuity-models/viewer/?url=../models/inception_v3/inception_v3.json
[Inception-v4]: https://hawk081.github.io/acuity-models/viewer/?url=../models/inception_v4/inception_v4.json
[Mobilenet-v1]: https://hawk081.github.io/acuity-models/viewer/?url=../models/mobilenet_v1/mobilenet_v1.json
[Mobilenet-v2]: https://hawk081.github.io/acuity-models/viewer/?url=../models/mobilenet_v2/mobilenet_v2.json
[Mobilenet-v3]: https://hawk081.github.io/acuity-models/viewer/?url=../models/mobilenet_v3/mobilenet_v3.json
[EfficientNet]: https://hawk081.github.io/acuity-models/viewer/?url=../models/efficientnet_b0/efficientnet_b0.json
[EfficientNet (EdgeTPU)]: https://hawk081.github.io/acuity-models/viewer/?url=../models/efficientnet_edgetpu/efficientnet_edgetpu.json
[Nasnet-Large]: https://hawk081.github.io/acuity-models/viewer/?url=../models/nasnet_large/nasnet_large.json
[Nasnet-Mobile]: https://hawk081.github.io/acuity-models/viewer/?url=../models/nasnet_mobile/nasnet_mobile.json
[Resnet-50]: https://hawk081.github.io/acuity-models/viewer/?url=../models/resnet50/resnet50.json
[Resnext-50]: https://hawk081.github.io/acuity-models/viewer/?url=../models/resnext50/resnext50.json
[Senet-50]: https://hawk081.github.io/acuity-models/viewer/?url=../models/senet50/senet50.json
[Squeezenet]: https://hawk081.github.io/acuity-models/viewer/?url=../models/squeezenet/squeezenet.json
[VGG-16]: https://hawk081.github.io/acuity-models/viewer/?url=../models/vgg16/vgg16.json
[Xception]: https://hawk081.github.io/acuity-models/viewer/?url=../models/xception/xception.json
[Faster-RCNN-ZF]: https://hawk081.github.io/acuity-models/viewer/?url=../models/faster_rcnn_zf/faster_rcnn_zf.json
[Mobilenet-SSD]: https://hawk081.github.io/acuity-models/viewer/?url=../models/mobilenet_ssd/mobilenet_ssd.json
[Mobilenet-SSD-FPN]: https://hawk081.github.io/acuity-models/viewer/?url=../models/mobilenet_ssd_fpn/mobilenet_ssd_fpn.json
[MTCNN PNet]: https://hawk081.github.io/acuity-models/viewer/?url=../models/mtcnn/mtcnn_pnet.json 
[RNet]: https://hawk081.github.io/acuity-models/viewer/?url=../models/mtcnn/mtcnn_rnet.json
[ONet]: https://hawk081.github.io/acuity-models/viewer/?url=../models/mtcnn/mtcnn_onet.json
[LNet]: https://hawk081.github.io/acuity-models/viewer/?url=../models/mtcnn/mtcnn_lnet.json
[SSD]: https://hawk081.github.io/acuity-models/viewer/?url=../models/ssd/ssd.json 
[Tiny-YOLO]: https://hawk081.github.io/acuity-models/viewer/?url=../models/tiny_yolo/tiny_yolo.json
[YOLO-v1]: https://hawk081.github.io/acuity-models/viewer/?url=../models/yolo_v1/yolo_v1.json
[YOLO-v2]: https://hawk081.github.io/acuity-models/viewer/?url=../models/yolo_v2/yolo_v2.json
[YOLO-v3]: https://hawk081.github.io/acuity-models/viewer/?url=../models/yolo_v3/yolo_v3.json
[ENET]: https://hawk081.github.io/acuity-models/viewer/?url=../models/enet/enet.json
[SegNet]: https://hawk081.github.io/acuity-models/viewer/?url=../models/segnet/segnet.json
[DeepLab-v3]: https://hawk081.github.io/acuity-models/viewer/?url=../models/deeplab_v3/deeplab_v3.json
[Denoiser]: https://hawk081.github.io/acuity-models/viewer/?url=../models/denoise/denoise.json
[Super Resolution]: https://hawk081.github.io/acuity-models/viewer/?url=../models/vdsr/vdsr.json
[Fast Style Transfer]: https://hawk081.github.io/acuity-models/viewer/?url=../models/fast_style_transfer/fast_style_transfer.json
[Pix2Pix]: https://hawk081.github.io/acuity-models/viewer/?url=../models/pix2pix/pix2pix.json
[Open Pose]: https://hawk081.github.io/acuity-models/viewer/?url=../models/open_pose/open_pose.json
[CPM Mobile]: https://hawk081.github.io/acuity-models/viewer/?url=../models/cpm/cpm.json
[LSTM - Command Recognition]: https://hawk081.github.io/acuity-models/viewer/?url=../models/lstm/lstm.json
[LSTM - Speech Recognition]: https://hawk081.github.io/acuity-models/viewer/?url=../models/deepspeech2/deepspeech2.json

[OriginAlexNet]: https://github.com/BVLC/caffe/tree/master/models/bvlc_alexnet
[OriginInception-v1]: http://download.tensorflow.org/models/inception_v1_2016_08_28.tar.gz
[OriginInception-v2]: http://download.tensorflow.org/models/inception_v2_2016_08_28.tar.gz
[OriginInception-v3]: http://download.tensorflow.org/models/inception_v3_2016_08_28.tar.gz
[OriginInception-v4]: http://download.tensorflow.org/models/inception_v4_2016_09_09.tar.gz
[OriginMobilenet-v1]: http://download.tensorflow.org/models/mobilenet_v1_2018_02_22/mobilenet_v1_1.0_224.tgz
[OriginMobilenet-v2]: https://storage.googleapis.com/mobilenet_v2/checkpoints/mobilenet_v2_1.0_224.tgz
[OriginMobilenet-v3]: https://storage.googleapis.com/mobilenet_v3/checkpoints/v3-large_224_1.0_float.tgz
[OriginEfficientNet]: https://storage.googleapis.com/cloud-tpu-checkpoints/efficientnet/ckpts/efficientnet-b0.tar.gz
[OriginEfficientNet-EdgeTPU]: https://github.com/tensorflow/tpu/tree/master/models/official/efficientnet/edgetpu
[OriginNasnet-Large]: https://storage.googleapis.com/download.tensorflow.org/models/nasnet-a_large_04_10_2017.tar.gz
[OriginNasnet-Mobile]: https://storage.googleapis.com/download.tensorflow.org/models/nasnet-a_mobile_04_10_2017.tar.gz
[OriginResnet-50]: http://download.tensorflow.org/models/resnet_v1_50_2016_08_28.tar.gz
[OriginResnext-50]: https://dl.fbaipublicfiles.com/resnext/imagenet_models/resnext_50_32x4d.t7
[OriginSenet-50]: https://github.com/hujie-frank/SENet
[OriginSqueezenet]: https://github.com/BVLC/caffe/wiki/Model-Zoo#squeezenet-alexnet-level-accuracy-with-50x-fewer-parameters
[OriginVGG-16]: http://download.tensorflow.org/models/vgg_16_2016_08_28.tar.gz
[OriginXception]: https://drive.google.com/file/d/1sJCRDhaNaJAnouKKulB3YO8Hu3q91KjP/view?usp=sharing
[OriginFaster-RCNN-ZF]: https://github.com/rbgirshick/fast-rcnn#extra-downloads
[OriginMobilenet-SSD]: http://download.tensorflow.org/models/object_detection/ssd_mobilenet_v1_coco_2018_01_28.tar.gz
[OriginMobilenet-SSD-FPN]: http://download.tensorflow.org/models/object_detection/ssd_mobilenet_v1_fpn_shared_box_predictor_640x640_coco14_sync_2018_07_03.tar.gz
[OriginMTCNN PNet]: https://github.com/imistyrain/MTCNN/tree/master/model/caffe
[OriginRNet]: https://github.com/imistyrain/MTCNN/tree/master/model/caffe
[OriginONet]: https://github.com/imistyrain/MTCNN/tree/master/model/caffe
[OriginLNet]: https://github.com/imistyrain/MTCNN/tree/master/model/caffe
[OriginSSD]: https://github.com/weiliu89/caffe/tree/ssd#models
[OriginTiny-YOLO]: https://drive.google.com/file/d/14-5ZojD1HSgMKnv6_E3WUcBPxaVm52X2/view?usp=sharing
[OriginYOLO-v1]: https://pjreddie.com/media/files/yolov1.weights
[OriginYOLO-v2]: https://pjreddie.com/media/files/yolov2.weights
[OriginYOLO-v3]: https://pjreddie.com/media/files/yolov3.weights
[OriginENET]: https://github.com/TimoSaemann/ENet
[OriginSegNet]: https://github.com/BVLC/caffe/wiki/Model-Zoo#segnet-and-bayesian-segnet
[OriginDeepLab-v3]: https://github.com/tensorflow/models/tree/master/research/deeplab
[OriginSuper Resolution]: https://github.com/tegg89/SRCNN-Tensorflow/tree/master/checkpoint/srcnn_21
[OriginFast Style Transfer]: https://drive.google.com/drive/folders/0B9jhaT37ydSyRk9UX0wwX3BpMzQ?usp=sharing
[OriginPix2Pix]: https://github.com/affinelayer/pix2pix-tensorflow
[OriginOpen Pose]: https://github.com/CMU-Perceptual-Computing-Lab/openpose
[OriginCPM Mobile]: https://drive.google.com/open?id=1gOwBY5puCusYPCQaPcEUMmQtPnGHCPyl
[OriginLSTM - Speech Recognition]: https://github.com/tensorflow/models/tree/master/research/deep_speech
