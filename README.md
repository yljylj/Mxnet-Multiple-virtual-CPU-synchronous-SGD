# Mxnet-Multiple-virtual-CPU-synchronous-SGD-on-Intel-platform
Devide the physical CPU to multiple virtual CPU, then doing a synchronous SGD. This method can speed up classification network training on Intel CPU. In addition, this method can also be applied to arm.

For example, if the CPU has 28 cores, we can divide it into 4 groups each with 7 cores and do a synchronos SGD. We do experiments On INTEL XEON E5-2690 v4 & INTEL XEON PLATINUM 8180 CPU, which can both get a 1.5x speed up when training Resnet or Mobilenet.

To run this, you need to cover original file on Mxnet.
