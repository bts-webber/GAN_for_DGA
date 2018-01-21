GAN for DGA
====


* 说明

> 试图使用生成对抗网络生成DGA域名，希望生成的域名不具备随机性，能够不被一些检测随机性的模型甄别出。
> 但这是似乎是一个失败的实验，鉴别器D用于鉴别域名是否是DGA和是否是机器生成的域名，训练数据使用的360DGA和top-1m,最终的生成器生成的域名类似于jjjjjjj.com这样重复的简单域名。

* RUN

> 1. 运行 D.py对鉴别器进行预训练。
> 2. 域名 G.py对生成器和鉴别器进行对抗训练。每隔20轮会打印出生成的前10个域名。
