# AP-BSN_demo01
这是一个AP-BSN去噪方法的本地复现和模型训练。环境配置与论文相同，代码在master分支下。
# 测试
在ckpt文件夹中有论文中已经训练好的APBSN_SIDD.pth模型，conf文件夹中有论文自带的APBSN_SIDD.yaml配置文件，数据集存放在dataset/strip目录下，运行以下命令完成测试：   
```python test.py -c APBSN_SIDD -g 0 --pretrained "D:/python-learning/AP-BSN/ckpt/APBSN_SIDD.pth" --test_dir "./dataset/strip/ColoredMosaic/5/```
# 训练
需准备 1.数据集 2.配置文件 3.数据处理模型。  
其中数据集存放在dataset目录下，配置文件存放在conf目录下，数据处理模型存放在src/datahandler/目录下，运行以下命令进行训练：  
```python train.py -c APBSN_Blue -g 0```

