# make-ipinyou-data_py3

**简体中文 | [English](README.md)**

这个项目是为了将 iPinYou 实时竞价数据使用 Python3 形式化为标准格式，以便进一步研究。下面我会给一个简洁明了的指引。

## Step 0

首先从百度网盘上下载数据集: [http://pan.baidu.com/s/1kTwX2mF](http://pan.baidu.com/s/1kTwX2mF)，UCL的链接失效了，不过百度网盘即使限速，一晚上差不多也下完了。

然后你会得到文件夹 `ipinyou.contest.dataset`，假设它的路径是  `~/ipinyou.contest.dataset`。

## Step 1

从 [wnzhang/make-ipinyou-data](https://github.com/wnzhang/make-ipinyou-data) 下载 `make-ipinyou-data`。

## Step 2

更新 `original-data` 中 `ipinyou.contest.dataset` 的软链接。

```shell
ln -sfn ~/ipinyou.contest.dataset ipinyou.contest.dataset
```

## Step 3

使用本仓库的替换其中的文件夹 `python` 。确保他们的权限是 775 或 777。

## Step 4

在 `make-ipinyou-data` 文件夹下，运行 `make all`。大约要花费30分钟，然后你就会得到：

```shell
859M    ./3358
482M    ./2259
1.3G    ./3427
1.4G    ./3386
56K    ./python
5.4G    ./all
1.6G    ./1458
396M    ./2261
804K    ./.git
1.1G    ./3476
4.0K    ./original-data
135M    ./2997
776M    ./2821
14G    .
```

更多关于数据集的细节，可以参考 [wnzhang/make-ipinyou-data](https://github.com/wnzhang/make-ipinyou-data)。