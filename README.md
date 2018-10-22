# CNN-models-comparison
The goal of this repository is:
- To keep on track of **state-of-the-art (SoTA)** and new CNN architectures
- To see the comparison of famous CNN models at a glance (accuracy, parameters, speed ...)
- To access their research papers and implementations on different frameworks

(This repository will be updated regularly.)

## Comparison Table
CNN model comparison table on the [ImageNet](http://www.image-net.org/) classification results, reference paper and implementations.

Model | Detail | Inpus size | Parameters | Mult-Adds | FLOPS | Depth | Top-1 Acc | Top-5 Acc | Paper | TF | Keras | Pytorch | Caffe | Torch | MXNet
-- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | --
AmoebaNet-B | (N=6, F=228) | 331x331⁵ | 155.3M⁵ | 41.1B⁵ |   |   | 83.10⁵ | 96.30⁵ | [Paper](https://arxiv.org/abs/1802.01548) | [TF](https://github.com/tensorflow/tpu/tree/master/models/official/amoeba_net) | - | - | - | - | -
PNASNet-5_Large_331 | (N=4, F=216) | 331x331⁵ | 86.1M⁵ | 25.0B⁵ |   |   | 82.90⁵ | 96.20⁵ | [Paper](https://arxiv.org/abs/1712.00559) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | - | - | - | - | -
AmoebaNet-B | (N=6, F=190) | 331x331⁵ | 86.7M⁵ | 23.1B⁵ |   |   | 82.80⁵ | 96.10⁵ | [Paper](https://arxiv.org/abs/1802.01548) | [TF](https://github.com/tensorflow/tpu/tree/master/models/official/amoeba_net) | - | - | - | - | -
SENet-154 |   | 320x320⁵ | 145.8M⁵ | 42.3B⁵ |   |   | 82.70⁵ | 96.20⁵ | [Paper](https://arxiv.org/pdf/1709.01507.pdf) | [TF](https://github.com/kobiso/SENet-tensorflow-slim) | [Keras](https://github.com/titu1994/keras-squeeze-excite-network) | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | [Caffe](https://github.com/hujie-frank/SENet) | - | -
NASNet-A_Large_331 | (N=6, F=168) | 331x331⁵ | 88.9M⁵ | 23.8B⁵ |   |   | 82.70⁵ | 96.20⁵ | [Paper](https://arxiv.org/abs/1707.07012) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/wandering007/nasnet-pytorch) | - | - | -
AmoebaNet-B | (N=6, F=190) | 331x331⁵ | 84.0M⁵ | 22.3B⁵ |   |   | 82.30⁵ | 96.10⁵ | [Paper](https://arxiv.org/abs/1802.01548) | [TF](https://github.com/tensorflow/tpu/tree/master/models/official/amoeba_net) | - | - | - | - | -
Dual-Path-Net-131 |   | 320x320⁵ | 79.5M⁵ | 32.0B⁵ |   |   | 81.50⁵ | 95.80⁵ | [Paper](https://arxiv.org/abs/1707.01629) | - | [Keras](https://github.com/titu1994/Keras-DualPathNetworks) | [Pytorch](https://github.com/Queequeg92/DualPathNet) | [Caffe](https://github.com/cypw/DPNs) | - | [MXNet](https://github.com/cypw/DPNs)
PolyNet |   | 331x331⁵ | 92M⁵ | 34.7B⁵ |   |   | 81.30⁵ | 95.80⁵ | [Paper](https://arxiv.org/abs/1611.05725) | - | - | [Pytorch](https://github.com/Cadene/pretrained-models.pytorch/blob/master/pretrainedmodels/models/polynet.py) | [Caffe](https://github.com/CUHK-MMLAB/polynet) | - | -
ResNeXt-101 | (64x4d) | 320x320⁵ | 83.6M⁵ | 31.5B⁵ |   |   | 80.90⁵ | 95.60⁵ | [Paper](https://arxiv.org/abs/1611.05431) | [TF](https://github.com/taki0112/ResNeXt-Tensorflow) | [Keras](https://github.com/titu1994/Keras-ResNeXt) | [Pytorch](https://github.com/prlz77/ResNeXt.pytorch) | [Caffe](https://github.com/cypw/ResNeXt-1) | [Torch](https://github.com/facebookresearch/ResNeXt) | -
PyramidNet-200 | α=300 | 320x320⁷ | 116.4M⁷ |   |   |   | 80.80⁷ | 95.30⁷ | [Paper](https://arxiv.org/abs/1610.02915.pdf) | [TF](https://github.com/yselivonchyk/Tensorflow_DeepPyramidalResidualNet) | - | [Pytorch](https://github.com/dyhan0920/PyramidNet-PyTorch) | [Caffe](https://github.com/jhkim89/PyramidNet-caffe) | [Torch](https://github.com/jhkim89/PyramidNet) | -
PyramidNet-200 | α=300 | 320x320⁷ | 62.1M⁷ |   |   |   | 80.50⁷ | 95.20⁷ | [Paper](https://arxiv.org/abs/1610.02915.pdf) | [TF](https://github.com/yselivonchyk/Tensorflow_DeepPyramidalResidualNet) | - | [Pytorch](https://github.com/dyhan0920/PyramidNet-PyTorch) | [Caffe](https://github.com/jhkim89/PyramidNet-caffe) | [Torch](https://github.com/jhkim89/PyramidNet) | -
Inception-ResNet-v2 |   | 299x299¹ | 55.8M² |   | 11.75G⁴ | 572² | 80.40¹ | 95.30¹ | [Paper](http://arxiv.org/abs/1602.07261) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://keras.io/applications/) | - | [Caffe](https://github.com/twtygqyy/Inception-resnet-v2) | - | -
Inception-ResNet-v2+SE |   | 299X299⁴ |   |   | 11.76G⁴ |   | 80.20⁴ | 95.21⁴ | [Paper](https://arxiv.org/pdf/1709.01507.pdf) | [TF](https://github.com/kobiso/SENet-tensorflow-slim) | - | [Pytorch](https://github.com/moskomule/senet.pytorch) | [Caffe](https://github.com/hujie-frank/SENet) | - | -
Inception V4 |   | 299x299¹ | 46M¹ |   |   |   | 80.20¹ | 95.20¹ | [Paper](http://arxiv.org/abs/1602.07261) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://github.com/kentsommer/keras-inceptionV4) | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | - | - | -
ResNet V2 200 |   | 320x320 | 64.7M |   | 15G |   | 79.90¹ | 95.20¹ | [Paper](https://arxiv.org/abs/1603.05027) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://github.com/raghakot/keras-resnet) | - | [Caffe](https://github.com/soeaver/caffe-model/tree/master/cls/resnet-v2) | - | -
bl-ResNet-152@256 | α=2, β=4 | 256x256⁸ | 57.36M⁸ |   | 6.58G⁸ |   | 79.66⁸ | - | [Paper](https://arxiv.org/abs/1807.03848) | - | - | - | - | - | -
bl-ResNeXt-101@256 | α=2, β=4 | 256x256⁸ | 41.51M⁸ |   | 5.33G⁸ |   | 79.59⁸ | - | [Paper](https://arxiv.org/abs/1807.03848) | - | - | - | - | - | -
bl-ResNet-152 | α=2, β=2 | 224x224⁸ | 59.81M⁸ |   | 5.64G⁸ |   | 79.04⁸ | - | [Paper](https://arxiv.org/abs/1807.03848) | - | - | - | - | - | -
Xception |   | 299x299² | 23M² |   |   | 126² | 79.00² | 94.50² | [Paper](https://arxiv.org/abs/1610.02357) | [TF](https://github.com/kwotsin/TensorFlow-Xception) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/tstandley/Xception-PyTorch) | [Caffe](https://github.com/yihui-he/Xception-caffe) | - | -
bl-ResNet-101@256 | α=2, β=4 | 256x256⁸ | 41.85M⁸ |   | 5.08G⁸ |   | 78.96⁸ | - | [Paper](https://arxiv.org/abs/1807.03848) | - | - | - | - | - | -
ResNeXt-101+CBAM | (32x4d) | 224x224³ | 49M³ |   | 7.519G³ |   | 78.93³ | 94.41³ | [Paper](https://arxiv.org/pdf/1807.06521.pdf) | [TF](https://github.com/kobiso/CBAM-tensorflow) | [Keras](https://github.com/kobiso/CBAM-keras) | - | - | - | -
bl-ResNet-152 | α=2, β=4 | 224x224⁸ | 57.36M⁸ |   | 5.04G⁸ |   | 78.84⁸ | - | [Paper](https://arxiv.org/abs/1807.03848) | - | - | - | - | - | -
ResNeXt-101+SE | (32x4d) | 224x224³ | 49M³ |   | 7.512G³ |   | 78.83³ | 94.34³ | [Paper](https://arxiv.org/pdf/1709.01507.pdf) | [TF](https://github.com/taki0112/SENet-Tensorflow) | - | - | [Caffe](https://github.com/hujie-frank/SENet) | - | -
bl-ResNeXt-101 | α=2, β=4 | 224x224⁸ | 41.51M⁸ |   | 4.08G⁸ |   | 78.80⁸ | - | [Paper](https://arxiv.org/abs/1807.03848) | - | - | - | - | - | -
bl-ResNeXt-50@256 | α=2, β=4 | 256x256⁸ | 26.19M⁸ |   | 3.95G⁸ |   | 78.77⁸ | - | [Paper](https://arxiv.org/abs/1807.03848) | - | - | - | - | - | -
bl-ResNet-101 | α=2, β=2 | 224x224⁸ | 43.39M⁸ |   | 4.27G⁸ |   | 78.60⁸ | - | [Paper](https://arxiv.org/abs/1807.03848) | - | - | - | - | - | -
ResNet101+CBAM |   | 224x224³ | 49M³ |   | 7.581G³ |   | 78.49³ | 94.31³ | [Paper](https://arxiv.org/pdf/1807.06521.pdf) | [TF](https://github.com/kobiso/CBAM-tensorflow-slim) | [Keras](https://github.com/kobiso/CBAM-keras) | - | - | - | -
ResNeXt-101 | (32x4d) | 224x224³ | 44.2M³ |   | 7.508G³ |   | 78.46³ | 94.25³ | [Paper](https://arxiv.org/abs/1611.05431) | [TF](https://github.com/taki0112/ResNeXt-Tensorflow) | [Keras](https://github.com/titu1994/Keras-ResNeXt) | [Pytorch](https://github.com/prlz77/ResNeXt.pytorch) | [Caffe](https://github.com/cypw/ResNeXt-1) | [Torch](https://github.com/facebookresearch/ResNeXt) | -
bl-ResNet-101 | α=2, β=4 | 224x224⁸ | 41.85M⁸ |   | 3.89G⁸ |   | 78.20⁸ | - | [Paper](https://arxiv.org/abs/1807.03848) | - | - | - | - | - | -
ResNeXt50+SE | (32x4d) | 224x224³ | 27.6M³ |   | 3.771G³ |   | 78.09³ | 93.96³ | [Paper](https://arxiv.org/pdf/1709.01507.pdf) | [TF](https://github.com/taki0112/SENet-Tensorflow) | - | - | [Caffe](https://github.com/hujie-frank/SENet) | - | -
ResNeXt50+CBAM | (32x4d) | 224x224³ | 27.6M³ |   | 3.774G³ |   | 78.08³ | 94.09³ | [Paper](https://arxiv.org/pdf/1807.06521.pdf) | [TF](https://github.com/kobiso/CBAM-tensorflow) | [Keras](https://github.com/kobiso/CBAM-keras) | - | - | - | -
bl-ResNeXt-50 | α=2, β=4 | 224x224⁸ | 26.19M⁸ |   | 3.03G⁸ |   | 78.00⁸ | - | [Paper](https://arxiv.org/abs/1807.03848) | - | - | - | - | - | -
Inception V3 |   | 299x299¹ | 23.8M² |   |   | 159² | 78.00¹ | 93.90¹ | [Paper](http://arxiv.org/abs/1512.00567) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | [Caffe](https://github.com/smichalowski/google_inception_v3_for_caffe) | - | -
ResNet V2 152 |   | 299x299¹ |   |   |   |   | 77.80¹ | 94.10¹ | [Paper](https://arxiv.org/abs/1603.05027) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://github.com/raghakot/keras-resnet) | - | [Caffe](https://github.com/soeaver/caffe-model/tree/master/cls/resnet-v2) | - | -
ResNet101+SE |   | 224x224³ | 49M³ |   | 7.575G³ |   | 77.65³ | 93.81³ | [Paper](https://arxiv.org/pdf/1709.01507.pdf) | [TF](https://github.com/kobiso/SENet-tensorflow-slim) | - | [Pytorch](https://github.com/moskomule/senet.pytorch) | [Caffe](https://github.com/hujie-frank/SENet) | - | -
ResNet50+CBAM |   | 224x224³ | 28M³ |   | 3.864G³ |   | 77.34³ | 93.69³ | [Paper](https://arxiv.org/pdf/1807.06521.pdf) | [TF](https://github.com/kobiso/CBAM-tensorflow-slim) | [Keras](https://github.com/kobiso/CBAM-keras) | - | - | - | -
bl-ResNet-50 | α=2, β=4 | 224x224⁸ | 26.69M⁸ |   | 2.85G⁸ |   | 77.31⁸ | - | [Paper](https://arxiv.org/abs/1807.03848) | - | - | - | - | - | -
ResNeXt50 | (32x4d) | 224x224³ | 25M³ |   | 3.768G³ |   | 77.15³ | 94.25³ | [Paper](https://arxiv.org/abs/1611.05431) | [TF](https://github.com/taki0112/ResNeXt-Tensorflow) | [Keras](https://github.com/titu1994/Keras-ResNeXt) | [Pytorch](https://github.com/prlz77/ResNeXt.pytorch) | [Caffe](https://github.com/cypw/ResNeXt-1) | [Torch](https://github.com/facebookresearch/ResNeXt) | -
DenseNet201 |   | 224x224² | 20M² |   |   | 201² | 77.00² | 93.30² | [Paper](https://arxiv.org/abs/1608.06993) | [TF](https://github.com/YixuanLi/densenet-tensorflow) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | [Caffe](https://github.com/shicai/DenseNet-Caffe) | - | -
ResNet V2 101 |   | 299x299¹ |   |   |   |   | 77.00¹ | 93.70¹ | [Paper](https://arxiv.org/abs/1603.05027) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://github.com/raghakot/keras-resnet) | - | [Caffe](https://github.com/soeaver/caffe-model/tree/master/cls/resnet-v2) | - | -
ResNet50+SE |   | 224x224³ | 28M³ |   | 3.86G³ |   | 76.86³ | 93.30³ | [Paper](https://arxiv.org/pdf/1709.01507.pdf) | [TF](https://github.com/kobiso/SENet-tensorflow-slim) | - | [Pytorch](https://github.com/moskomule/senet.pytorch) | [Caffe](https://github.com/hujie-frank/SENet) | - | -
bl-ResNet-50 | α=4, β=4 | 224x224⁸ | 26.24M⁸ |   | 2.48G⁸ |   | 76.85⁸ | - | [Paper](https://arxiv.org/abs/1807.03848) | - | - | - | - | - | -
ResNet V1 152 |   | 224x224¹ | 60M |   | 11.3G⁴ | 517 | 76.80¹ | 93.20¹ | [Paper](https://arxiv.org/abs/1512.03385) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://github.com/statech/resnet) | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | [Caffe](https://github.com/KaimingHe/deep-residual-networks) | [Torch](https://github.com/facebook/fb.resnet.torch) | -
ResNet V1 101 |   | 224x224¹ | 45M³ |   | 7.57G³ |   | 76.40¹ | 92.90¹ | [Paper](https://arxiv.org/abs/1512.03385) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://github.com/statech/resnet) | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | [Caffe](https://github.com/KaimingHe/deep-residual-networks) | [Torch](https://github.com/facebook/fb.resnet.torch) | -
MnasNet-92+SE |   | 224x224⁹ | 5.1M⁹ | 391M⁹ |   |   | 76.13⁹ | 92.85⁹ | [Paper](https://arxiv.org/abs/1807.11626) | [TF](https://github.com/Lyken17/MNasNet-TensorFlow) | [Keras](https://github.com/abhoi/Keras-MnasNet) | [Pytorch](https://github.com/AnjieZheng/MnasNet-PyTorch) | [Caffe](https://github.com/LiJianfei06/MnasNet-caffe) | - | -
DenseNet169 |   | 224x224² | 14M² |   |   | 169² | 75.90² | 92.80² | [Paper](https://arxiv.org/abs/1608.06993) | [TF](https://github.com/YixuanLi/densenet-tensorflow) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | [Caffe](https://github.com/shicai/DenseNet-Caffe) | - | -
BN-Inception+SE |   | 224x224⁴ |   |   | 2.04G⁴ |   | 75.77⁴ | 92.86⁴ | [Paper](https://arxiv.org/pdf/1709.01507.pdf) | [TF](https://github.com/kobiso/SENet-tensorflow-slim) | - | - | [Caffe](https://github.com/hujie-frank/SENet) | - | -
ResNet V2 50 |   | 299x299¹ |   |   |   |   | 75.60¹ | 92.80¹ | [Paper](https://arxiv.org/abs/1603.05027) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://github.com/raghakot/keras-resnet) | - | [Caffe](https://github.com/soeaver/caffe-model/tree/master/cls/resnet-v2) | - | -
MnasNet+SE |   | 224x224⁹ | 4.7M⁹ | 319M⁹ |   |   | 75.42⁹ | 92.51⁹ | [Paper](https://arxiv.org/abs/1807.11626) | [TF](https://github.com/Lyken17/MNasNet-TensorFlow) | [Keras](https://github.com/abhoi/Keras-MnasNet) | [Pytorch](https://github.com/AnjieZheng/MnasNet-PyTorch) | [Caffe](https://github.com/LiJianfei06/MnasNet-caffe) | - | -
ResNet V1 50 |   | 224x224¹ | 25.6M² |   | 3.858G³ | 168² | 75.20¹ | 92.20¹ | [Paper](https://arxiv.org/abs/1512.03385) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | [Caffe](https://github.com/KaimingHe/deep-residual-networks) | [Torch](https://github.com/facebook/fb.resnet.torch) | -
WideResNet18+CBAM | widen=2.0 | 224x224³ | 45.97M³ |   | 6.697G³ |   | 75.16³ | 92.37³ | [Paper](https://arxiv.org/pdf/1807.06521.pdf) | - | - | - | - | - | -
WideResNet18+SE | widen=2.0 | 224x224³ | 45.97M³ |   | 6.696G³ |   | 75.07³ | 92.35³ | [Paper](https://arxiv.org/pdf/1709.01507.pdf) | - | - | - | [Caffe](https://github.com/hujie-frank/SENet) | - | -
MobileNet_v2 | α=1.4 | 224x224¹ | 6M |   |   |   | 74.90¹ | 92.50¹ | [Paper](https://arxiv.org/abs/1801.04381) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/tonylins/pytorch-mobilenet-v2) | [Caffe](https://github.com/shicai/MobileNet-Caffe) | - | -
MnasNet-92 |   | 224x224⁹ | 4.4M⁹ | 388M⁹ |   |   | 74.79⁹ | 92.05⁹ | [Paper](https://arxiv.org/abs/1807.11626) | [TF](https://github.com/Lyken17/MNasNet-TensorFlow) | [Keras](https://github.com/abhoi/Keras-MnasNet) | [Pytorch](https://github.com/AnjieZheng/MnasNet-PyTorch) | [Caffe](https://github.com/LiJianfei06/MnasNet-caffe) | - | -
MnasNet-65+SE |   | 224x224⁹ | 4.1M⁹ | 272M⁹ |   |   | 74.62⁹ | 91.93⁹ | [Paper](https://arxiv.org/abs/1807.11626) | [TF](https://github.com/Lyken17/MNasNet-TensorFlow) | [Keras](https://github.com/abhoi/Keras-MnasNet) | [Pytorch](https://github.com/AnjieZheng/MnasNet-PyTorch) | [Caffe](https://github.com/LiJianfei06/MnasNet-caffe) | - | -
BN-Inception |   | 224x224⁴ |   |   | 2.03G⁴ |   | 74.62⁴ | 92.21⁴ | [Paper](https://arxiv.org/pdf/1502.03167) | - | - | - | [Caffe](https://github.com/pertusa/InceptionBN-21K-for-Caffe) | - | -
AmoebaNet-A |   | 224x224⁹ | 5.1M⁹ | 555M⁹ |   |   | 74.50⁹ | 92.00⁹ | [Paper](https://arxiv.org/abs/1802.01548) | [TF](https://github.com/tensorflow/tpu/tree/master/models/official/amoeba_net) | - | - | - | - | -
DenseNet121 |   | 224x224² | 8M² |   |   | 121² | 74.50² | 91.80² | [Paper](https://arxiv.org/abs/1608.06993) | [TF](https://github.com/YixuanLi/densenet-tensorflow) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | [Caffe](https://github.com/shicai/DenseNet-Caffe) | - | -
WideResNet18 | widen=2.0 | 224x224³ | 45.62M³ |   | 6.696G³ |   | 74.37³ | 91.80³ | [Paper](https://arxiv.org/abs/1605.07146) | [TF](https://github.com/dalgu90/wrn-tensorflow) | [Keras](https://github.com/titu1994/Wide-Residual-Networks) | [Pytorch](https://github.com/xternalz/WideResNet-pytorch) | [Caffe](https://github.com/razorx89/caffe-wrn-generator) | - | -
PNASNet-5_Mobile |   | 224x224⁹ | 5.1M⁹ | 588M⁹ |   |   | 74.20⁹ | 91.90⁹ | [Paper](https://arxiv.org/abs/1712.00559.pdf) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | - | - | - | - | -
ResNet34+CBAM |   | 224x224³ | 22M³ |   | 3.665G³ |   | 74.01³ | 91.76³ | [Paper](https://arxiv.org/pdf/1807.06521.pdf) | [TF](https://github.com/kobiso/CBAM-tensorflow-slim) | [Keras](https://github.com/kobiso/CBAM-keras) | - | - | - | -
MnasNet |   | 224x224⁹ | 4.2M⁹ | 317M⁹ |   |   | 74.00⁹ | 91.78⁹ | [Paper](https://arxiv.org/abs/1807.11626) | [TF](https://github.com/Lyken17/MNasNet-TensorFlow) | [Keras](https://github.com/abhoi/Keras-MnasNet) | [Pytorch](https://github.com/AnjieZheng/MnasNet-PyTorch) | [Caffe](https://github.com/LiJianfei06/MnasNet-caffe) | - | -
NASNet-A_Mobile_224 |   | 224x224¹ |   |   |   |   | 74.00¹ | 91.60¹ | [Paper](https://arxiv.org/abs/1707.07012) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/wandering007/nasnet-pytorch) | - | - | -
WideResNet18+CBAM | widen=1.5 | 224x224³ | 26.08M³ |   | 3.868G³ |   | 73.90³ | 91.57³ | [Paper](https://arxiv.org/pdf/1807.06521.pdf) | - | - | - | - | - | -
Inception V2 |   | 224x224¹ |   |   |   |   | 73.90¹ | 91.80¹ | [Paper](http://arxiv.org/abs/1502.03167) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | - | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | - | - | -
ResNet34+SE |   | 224x224³ | 22M³ |   | 3.664G³ |   | 73.87³ | 91.65³ | [Paper](https://arxiv.org/pdf/1709.01507.pdf) | [TF](https://github.com/kobiso/SENet-tensorflow-slim) | - | [Pytorch](https://github.com/moskomule/senet.pytorch) | [Caffe](https://github.com/hujie-frank/SENet) | - | -
CondenseNet | G=C=8 | 224x224⁹ | 4.8M⁹ | 529M⁹ |   |   | 73.80⁹ | 91.70⁹ | [Paper](https://arxiv.org/abs/1711.09224) | [TF](https://github.com/markdtw/condensenet-tensorflow) | - | [Pytorch](https://github.com/ShichenLiu/CondenseNet) | - | - | -
WideResNet18+SE | widen=1.5 | 224x224³ | 26.07M³ |   | 3.867G³ |   | 73.79³ | 91.53³ | [Paper](https://arxiv.org/pdf/1709.01507.pdf) | - | - | - | [Caffe](https://github.com/hujie-frank/SENet) | - | -
ShuffleNet | x2 | 224x224⁹ | 5.4M⁹ | 524M⁹ |   |   | 73.70⁹ | - | [Paper](https://arxiv.org/abs/1707.01083) | [TF](https://github.com/MG2033/ShuffleNet) | [Keras](https://github.com/scheckmedia/keras-shufflenet) | [Pytorch](https://github.com/jaxony/ShuffleNet) | [Caffe](https://github.com/farmingyard/ShuffleNet) | - | -
ResNet34 |   | 224x224³ | 21.8M³ |   | 3.664G³ |   | 73.31³ | 91.40³ | [Paper](https://arxiv.org/abs/1512.03385) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | - | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | [Caffe](https://github.com/KaimingHe/deep-residual-networks) | [Torch](https://github.com/facebook/fb.resnet.torch) | -
WideResNet18 | widen=1.5 | 224x224³ | 25.88M³ |   | 3.866G³ |   | 73.15³ | 91.12³ | [Paper](https://arxiv.org/abs/1605.07146) | [TF](https://github.com/dalgu90/wrn-tensorflow) | [Keras](https://github.com/titu1994/Wide-Residual-Networks) | [Pytorch](https://github.com/xternalz/WideResNet-pytorch) | [Caffe](https://github.com/razorx89/caffe-wrn-generator) | - | -
DARTS |   | 224x224⁹ | 4.9M⁹ | 595M⁹ |   |   | 73.10⁹ | 91.00⁹ | [Paper](https://arxiv.org/abs/1806.09055) | - | - | [Pytorch](https://github.com/quark0/darts) | - | - | -
MnasNet-65 |   | 224x224⁹ | 3.6M⁹ | 270M⁹ |   |   | 73.02⁹ | 91.14⁹ | [Paper](https://arxiv.org/abs/1807.11626) | [TF](https://github.com/Lyken17/MNasNet-TensorFlow) | [Keras](https://github.com/abhoi/Keras-MnasNet) | [Pytorch](https://github.com/AnjieZheng/MnasNet-PyTorch) | [Caffe](https://github.com/LiJianfei06/MnasNet-caffe) | - | -
MobileNet_v2 | α=1.0 | 224x224¹ | 3.47M |   |   |   | 71.90¹ | 91.00¹ | [Paper](https://arxiv.org/abs/1801.04381) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/tonylins/pytorch-mobilenet-v2) | [Caffe](https://github.com/shicai/MobileNet-Caffe) | - | -
ShuffleNet | 1.5 | 224x224⁹ | 3.4M⁹ | 292M⁹ |   |   | 71.50⁹ | - | [Paper](https://arxiv.org/abs/1707.01083) | [TF](https://github.com/MG2033/ShuffleNet) | [Keras](https://github.com/scheckmedia/keras-shufflenet) | [Pytorch](https://github.com/jaxony/ShuffleNet) | [Caffe](https://github.com/farmingyard/ShuffleNet) | - | -
VGG 16 |   | 224x224¹ | 138M² |   | 15.47⁴ | 23² | 71.50¹ | 89.80¹ | [Paper](http://arxiv.org/abs/1409.1556.pdf) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | [Caffe](https://github.com/davidgengenbach/vgg-caffe) | - | -
VGG 19 |   | 224x224¹ | 143M² |   |   | 26² | 71.10¹ | 89.80¹ | [Paper](http://arxiv.org/abs/1409.1556.pdf) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | [Caffe](https://github.com/davidgengenbach/vgg-caffe) | - | -
CondenseNet | G=C=4 | 224x224⁹ | 2.9M⁹ | 274M⁹ |   |   | 71.00⁹ | 90.00⁹ | [Paper](https://arxiv.org/abs/1711.09224) | [TF](https://github.com/markdtw/condensenet-tensorflow) | - | [Pytorch](https://github.com/ShichenLiu/CondenseNet) | - | - | -
MobileNet_v1+CBAM | α=1.0 | 224x224³ | 5.07M³ |   | 0.576G³ |   | 70.99³ | 90.01³ | [Paper](https://arxiv.org/pdf/1807.06521.pdf) | - | [Keras](https://github.com/kobiso/CBAM-keras) | - | - | - | -
MobileNet_v1 | α=1.0 | 224x224¹ |   |   |   |   | 70.90¹ | 89.90¹ | [Paper](https://arxiv.org/pdf/1704.04861.pdf) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/marvis/pytorch-mobilenet) | [Caffe](https://github.com/shicai/MobileNet-Caffe) | - | -
ResNet18+CBAM |   | 224x224³ | 11.8M³ |   | 1.815G³ |   | 70.73³ | 89.91³ | [Paper](https://arxiv.org/pdf/1807.06521.pdf) | [TF](https://github.com/kobiso/CBAM-tensorflow-slim) | [Keras](https://github.com/kobiso/CBAM-keras) | - | - | - | -
ResNet18+SE |   | 224x224³ | 11.8M³ |   | 1.814G³ |   | 70.59³ | 89.78³ | [Paper](https://arxiv.org/pdf/1709.01507.pdf) | [TF](https://github.com/kobiso/SENet-tensorflow-slim) | - | [Pytorch](https://github.com/moskomule/senet.pytorch) | [Caffe](https://github.com/hujie-frank/SENet) | - | -
ResNet18 |   | 224x224³ | 11.7M³ |   | 1.814G³ |   | 70.40³ | 89.45³ | [Paper](https://arxiv.org/abs/1512.03385) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | - | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | [Caffe](https://github.com/KaimingHe/deep-residual-networks) | [Torch](https://github.com/facebook/fb.resnet.torch) | -
MobileNet_v1+SE | α=1.0 | 224x224³ | 5.07M³ |   | 0.570G³ |   | 70.03³ | 89.37³ | [Paper](https://arxiv.org/pdf/1709.01507.pdf) | - | - | - | [Caffe](https://github.com/hujie-frank/SENet) | - | -
Inception V1 |   | 224x224¹ |   |   |   |   | 69.80¹ | 89.60¹ | [Paper](http://arxiv.org/abs/1409.4842v1) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://gist.github.com/joelouismarino/a2ede9ab3928f999575423b9887abd14) | [Pytorch](https://github.com/pytorch/vision/tree/master/torchvision) | - | - | -
MobileNet_v1 | α=1.0 | 224x224³ | 4.23M³ |   | 0.569G³ |   | 68.61³ | 88.49³ | [Paper](https://arxiv.org/pdf/1704.04861.pdf) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/marvis/pytorch-mobilenet) | [Caffe](https://github.com/shicai/MobileNet-Caffe) | - | -
MobileNet_v1+CBAM | α=0.7 | 224x224³ | 2.71M³ |   | 0.289G³ |   | 68.49³ | 88.52³ | [Paper](https://arxiv.org/pdf/1807.06521.pdf) | - | [Keras](https://github.com/kobiso/CBAM-keras) | - | - | - | -
ShuffleNet+SE | 1x(g=3) | 224x224⁴ | 2.4M⁴ |   | 0.142G⁴ |   | 68.30⁴ | 88.30⁴ | [Paper](https://arxiv.org/pdf/1709.01507.pdf) | - | - | - | [Caffe](https://github.com/hujie-frank/SENet) | - | -
SqueezeNext |   | 224x224⁹ | 3.2M⁹ | 708M⁹ |   |   | 67.50⁹ | 88.20⁹ | [Paper](https://arxiv.org/abs/1803.10615) | [TF](https://github.com/Timen/squeezenext-tensorflow) | - | [Pytorch](https://github.com/luuuyi/SqueezeNext.PyTorch) | [Caffe](https://github.com/amirgholami/SqueezeNext) | - | -
MobileNet_v1+SE | α=0.7 | 224x224³ | 2.71M³ |   | 0.283G³ |   | 67.50³ | 87.51³ | [Paper](https://arxiv.org/pdf/1709.01507.pdf) | - | - | - | [Caffe](https://github.com/hujie-frank/SENet) | - | -
ShuffleNet | 1x(g=3) | 224x224⁴ | 1.8M⁴ |   | 0.14G⁴ |   | 66.10⁴ | 86.40⁴ | [Paper](https://arxiv.org/pdf/1707.01083) | [TF](https://github.com/MG2033/ShuffleNet) | [Keras](https://github.com/scheckmedia/keras-shufflenet) | [Pytorch](https://github.com/jaxony/ShuffleNet) | [Caffe](https://github.com/farmingyard/ShuffleNet) | - | -
MobileNet_v1 | α=0.7 | 224x224³ | 2.3M³ |   | 0.283G³ |   | 65.14³ | 86.31³ | [Paper](https://arxiv.org/pdf/1704.04861.pdf) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/marvis/pytorch-mobilenet) | [Caffe](https://github.com/shicai/MobileNet-Caffe) | - | -
MobileNet_v1 | α=0.5 | 160x160¹ |   |   |   |   | 59.10¹ | 81.90¹ | [Paper](https://arxiv.org/pdf/1704.04861.pdf) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/marvis/pytorch-mobilenet) | [Caffe](https://github.com/shicai/MobileNet-Caffe) | - | -
MobileNet_v1 | α=0.25 | 128x128¹ |   |   |   |   | 41.50¹ | 66.30¹ | [Paper](https://arxiv.org/pdf/1704.04861.pdf) | [TF](https://github.com/tensorflow/models/tree/master/research/slim) | [Keras](https://keras.io/applications/) | [Pytorch](https://github.com/marvis/pytorch-mobilenet) | [Caffe](https://github.com/shicai/MobileNet-Caffe) | - | -

- **Mult-Adds**: The number of multiply-add operations
- **FLOPS**: The floating point operations

### Value References
Superscript numbers on each value indicate the reference number of each value from.
1. [TF-Slim](https://github.com/tensorflow/models/tree/master/research/slim)
2. [Keras: Applications](https://keras.io/applications/)
3. [CBAM: Convolutional Block Attention Module](https://arxiv.org/abs/1807.06521.pdf)
4. [Squeeze-and-Excitation Networks](https://arxiv.org/abs/1709.01507.pdf)
5. [Progressive Neural Architecture Search](https://arxiv.org/abs/1712.00559.pdf)
6. [Residual Attention Network for Image Classification](https://arxiv.org/abs/1704.06904.pdf)
7. [Deep Pyramidal Residual Networks](https://arxiv.org/abs/1610.02915.pdf)
8. [Big-Little Net: An Efficient Multi-Scale Feature Representation for Visual and Speech Recognition](https://arxiv.org/abs/1807.03848)
9. [MnasNet: Platform-Aware Neural Architecture Search for Mobile](https://arxiv.org/abs/1807.11626)

## Related Resources
Check the other good resources about CNN models
- [Caffe-model](https://github.com/soeaver/caffe-model)
- [TensorNets](https://github.com/taehoonlee/tensornets)
- [DeepDetect : Open Source Deep Learning Server & API](https://github.com/jolibrain/deepdetect#deepdetect--open-source-deep-learning-server--api)
- [Pretrained models for Pytorch](https://github.com/Cadene/pretrained-models.pytorch)
- [Netscope CNN Analyzer](https://dgschwend.github.io/netscope/quickstart.html)
- [Memory consumption and FLOP count](https://github.com/albanie/convnet-burden)

## Author
Byung Soo Ko / kobiso62@gmail.com
