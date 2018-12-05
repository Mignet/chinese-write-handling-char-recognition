# chinese-write-handling-char-recognition
汉字手写识别

## 数据集
数据集来自于中科院自动化研究所，具体下载地址:
``http://www.nlpr.ia.ac.cn/databases/download/feature_data/HWDB1.1trn_gnt.zip``
``http://www.nlpr.ia.ac.cn/databases/download/feature_data/HWDB1.1tst_gnt.zip``

这个训练集和测试集是经过压缩的图片，需要解压出来转换图片，这里是转换好的文件包：https://pan.baidu.com/s/1o84jIrg

## 构建神经网络
![网络](https://github.com/Mignet/chinese-write-handling-char-recognition/blob/master/pic/png.png?raw=true)

## 训练
run the command ``python chinese_rec.py --mode=train --max_steps=16002 --eval_steps=100 --save_steps=500``

## 校验
run the command ``python chinese_rec.py --mode=validation``
![网络](https://raw.githubusercontent.com/Mignet/chinese-write-handling-char-recognition/master/pic/accuracy.svg)
## 测试
run the command ``python chinese_rec.py--mode=inference``


