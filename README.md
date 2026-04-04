# 使用GAN生成二次元头像

这是《PyTorch深度学习入门》(ISBN 978-7-115-51919-1)第六章的一个小项目

该项目基于生成对抗网络来生成二次元头像

## Structure

```
.
├── faces
├── faces.py                    # 使用一个基于opencv的工具截取头像
├── gan.ipynb                   # 训练程序
├── imgs
├── lbpcascade_animeface.xml    # 截取头像工具的依赖文件
├── README.md
└── reptile.ipynb               # 爬虫程序，从konachan.net获取二次元图片
```

## Guide

### 1. 运行reptile.ipynb获取图片
爬虫程序会从konachan.net网站上爬取动漫图片，并存入imgs文件夹中


### 2. 运行faces.py从获取的图片中截取头像
这个工具会将获取的动漫图片中的人物头像截取出来并存入imgs文件夹中
⚠️注意：在生成头像数据后需要手动将faces中的图片分进两个不同的文件夹中

### 3. 运行训练程序

## 声明与致谢

1. 该项目的代码和指导来自《PyTorch深度学习入门》曾芃壹 著
2. 训练GAN所需的图片数据来自<https://konachan.net>
3. 获取并处理图片使用的程序参考自[GAN学习生成指南：从原理入门到制作生成Demo](https://zhuanlan.zhihu.com/p/24767059)
4. 截取头像的工具是<https://github.com/nagadomi/lbpcascade_animeface>
5. **免责声明：** 本项目仅用于个人学习和研究，如有侵权请联系删除