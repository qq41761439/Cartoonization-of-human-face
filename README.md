# Cartoonization-of-human-face
本项目将人脸照片转换为卡通头像：使用到 **CycleGAN** 和 **G-means** 两种方法

## CycleGAN
CycleGAN 其实就是一个 A→B 单向 GAN 加上一个 B→A 单向 GAN。两个 GAN 共享两个生成器，然后各自带一个判别器，所以加起来总共有两个判别器和两个生成器。一个单向 GAN 有两个 loss，而 CycleGAN 加起来总共有四个 loss。  
CycleGAN 论文的原版原理图和公式如下：
