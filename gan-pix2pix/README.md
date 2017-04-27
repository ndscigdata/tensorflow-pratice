# tensorflow-pratice

对图像转图像之间的操作实验

需要包：opencv,
        scipy,
        matplotlib,
        numpy,
		tensorflow,
		tensorflow model
		
本实验主要参考代码为：https://github.com/affinelayer/pix2pix-tensorflow

（1）首先下载数据集，https://people.eecs.berkeley.edu/~tinghuiz/projects/pix2pix/datasets/，从这个网址上可以下载很多个经典的应用数据集。本文实验只选用facades这个数据集，由于剩下原理都是一样的。

（2）进行训练

在程序pix2pix.py代码中，手动添加测试参数，本文只让运行200次。

  # 训练的时候的参数

#     a.input_dir = "/home/ndscbigdata/work/imgdata/facades/train"
#     a.mode = "train"
#     a.output_dir = "/home/ndscbigdata/work/imgdata/facades/ckt"
#     a.max_epochs=200
#     a.which_direction = "BtoA"

（3）进行测试

　# 测试的时候的参数
    a.input_dir = "/home/ndscbigdata/work/imgdata/facades/val"
    a.mode = "test"
    a.output_dir = "/home/ndscbigdata/work/imgdata/facades/facades_test"
    a.checkpoint="/home/ndscbigdata/work/imgdata/facades/ckt"
	
	具体过程见博客：[CSDN博客](http://blog.csdn.net/sparkexpert/article/details/70837669)
