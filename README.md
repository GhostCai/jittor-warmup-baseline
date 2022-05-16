# Jittor 计图挑战热身赛 baseline


## 简介
本项目包含了第二届计图挑战赛计图 - 计图挑战热身赛的代码实现。主要在Conditional GAN的实例代码上进行了修改。

## 安装 
```bash
git clone https://gitlink.org.cn/GhostCai/jittor_warmup_baseline.git
```

本项目可在 1 张 2080Ti 上运行，训练时间约为 10分钟。

#### 运行环境
- ubuntu 20.04 LTS
- python = 3.7
- jittor = 1.3.0

#### 安装依赖
执行以下命令安装 python 依赖
```
pip install -r requirements.txt
```

#### 预训练模型
预训练模型`discriminator_last.pkl`和`generator_last.pkl`已经放在项目中。

## 训练
```python
python CGAN.py
```

## 推理
生成测试集上的结果可以运行以下命令：

```
python val.py --number '13503518888'
```

## 致谢
此项目基于[gan-jittor/competition at master · Jittor/gan-jittor (github.com)](https://github.com/Jittor/gan-jittor/tree/master/competition#计图挑战热身赛)实现，部分代码参考了 [jittor-gan](https://github.com/Jittor/gan-jittor)。

## 注意事项

点击项目的“设置”，在Description一栏中添加项目描述，需要包含“jittor”字样。同时在Topics中需要添加jittor。

![image-20220419164035639](https://s3.bmp.ovh/imgs/2022/04/19/6a3aa627eab5f159.png)